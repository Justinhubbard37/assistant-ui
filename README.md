## aui-perf nightly record

_3 points · 2026-11-13T12:30:39.442Z to 2026-11-15T12:09:15.182Z · latest runner: INTEL(R) XEON(R) PLATINUM 8573C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 581.52µs |  |  | 429.43µs | 859.20µs | 3 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 848.04µs |  |  | 657.87µs | 1.224ms | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 41.13µs |  |  | 30.56µs | 56.85µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 475.75µs |  |  | 361.89µs | 641.80µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 7.406ms |  |  | 5.568ms | 10.043ms | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 202.20µs |  |  | 148.79µs | 282.52µs | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.939ms |  |  | 1.370ms | 2.529ms | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 7.306ms |  |  | 5.512ms | 9.900ms | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.87µs |  |  | 5.16µs | 9.71µs | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 57.10µs |  |  | 43.60µs | 85.87µs | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 225.61µs |  |  | 168.77µs | 347.11µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 71.39µs |  |  | 50.90µs | 142.84µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 32.38µs |  |  | 23.77µs | 81.67µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 33.24µs |  |  | 26.20µs | 82.76µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 209.33µs |  |  | 149.36µs | 319.38µs | 3 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 53.15µs |  |  | 38.17µs | 75.45µs | 3 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 520.08µs |  |  | 359.63µs | 688.91µs | 3 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.12µs |  |  | 5.14µs | 10.18µs | 3 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 56.80µs |  |  | 45.08µs | 84.63µs | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 486.63µs |  |  | 367.93µs | 758.23µs | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.996ms |  |  | 3.247ms | 6.014ms | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 15.735ms |  |  | 12.796ms | 23.817ms | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 230.88µs |  |  | 190.34µs | 352.26µs | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.269ms |  |  | 1.873ms | 3.310ms | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.808ms |  |  | 7.286ms | 13.073ms | 3 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 189.79µs |  |  | 136.31µs | 274.11µs | 3 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.838ms |  |  | 794.22µs | 1.989ms | 3 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 48.59µs |  |  | 33.04µs | 68.04µs | 3 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 480.11µs |  |  | 343.49µs | 689.14µs | 3 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.512ms |  |  | 1.834ms | 3.677ms | 3 |
| external-message-conversion › core: external message tool results › 100 matches | 58.16µs |  |  | 37.37µs | 81.72µs | 3 |
| external-message-conversion › core: external message tool results › 1000 matches | 578.06µs |  |  | 384.57µs | 819.69µs | 3 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.032ms |  |  | 1.989ms | 4.221ms | 3 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 29.97µs |  |  | 20.26µs | 41.87µs | 3 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 285.61µs |  |  | 190.52µs | 411.84µs | 3 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.535ms |  |  | 1.041ms | 2.218ms | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.19µs |  |  | 0.14µs | 0.28µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.33µs |  |  | 0.24µs | 0.46µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.73µs |  |  | 1.42µs | 2.41µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.42µs |  |  | 0.34µs | 0.66µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.42µs |  |  | 1.63µs | 3.56µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 21.95µs |  |  | 14.96µs | 32.26µs | 3 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 123.44µs |  |  | 85.39µs | 153.69µs | 3 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 688.80µs |  |  | 436.67µs | 889.09µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.358ms |  |  | 1.327ms | 2.871ms | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 179.11µs |  |  | 97.31µs | 212.68µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 3.063ms |  |  | 1.744ms | 3.724ms | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 382.60µs |  |  | 243.79µs | 514.91µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 541.68µs |  |  | 351.48µs | 725.76µs | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 7.003ms |  |  | 3.741ms | 7.522ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 860.98µs |  |  | 441.49µs | 947.41µs | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 16.323ms |  |  | 10.454ms | 25.040ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.654ms |  |  | 1.727ms | 3.716ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.972ms |  |  | 1.367ms | 2.813ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.359ms |  |  | 1.455ms | 3.236ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.538ms |  |  | 1.662ms | 3.470ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 16.127ms |  |  | 10.846ms | 22.745ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 17.186ms |  |  | 12.252ms | 23.466ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.244ms |  |  | 758.93µs | 1.502ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.269ms |  |  | 1.446ms | 3.117ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.284ms |  |  | 5.340ms | 10.063ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.236ms |  |  | 1.145ms | 1.236ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.293ms |  |  | 1.178ms | 1.970ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.498ms |  |  | 2.946ms | 4.752ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 221.55µs |  |  | 174.54µs | 326.73µs | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.863ms |  |  | 1.543ms | 2.747ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 203.350ms |  |  | 142.981ms | 302.495ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 9.213ms |  |  | 7.502ms | 12.929ms | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.55µs |  |  | 1.22µs | 2.26µs | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.57µs |  |  | 5.57µs | 9.58µs | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 27.40µs |  |  | 17.49µs | 41.57µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 5.73µs |  |  | 4.42µs | 6.43µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 16.07µs |  |  | 12.94µs | 21.16µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 55.46µs |  |  | 44.35µs | 63.04µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 191.19µs |  |  | 175.04µs | 267.10µs | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.780ms |  |  | 3.376ms | 6.967ms | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 25.807ms |  |  | 23.023ms | 46.723ms | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 314.158ms |  |  | 314.158ms | 503.513ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 372.41µs |  |  | 240.55µs | 668.60µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 675.14µs |  |  | 391.88µs | 921.48µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.150ms |  |  | 1.837ms | 4.067ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 387.37µs |  |  | 253.67µs | 641.78µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.240ms |  |  | 734.91µs | 1.531ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 8.682ms |  |  | 6.328ms | 13.918ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 370.55µs |  |  | 230.48µs | 588.52µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 838.94µs |  |  | 495.91µs | 1.182ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.752ms |  |  | 3.532ms | 7.756ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 157.54µs |  |  | 109.91µs | 330.19µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 355.53µs |  |  | 243.26µs | 557.66µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.481ms |  |  | 1.596ms | 3.512ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 11.71µs |  |  | 8.63µs | 22.69µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 24.64µs |  |  | 18.83µs | 41.60µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 204.79µs |  |  | 125.87µs | 271.30µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 426.74µs |  |  | 261.56µs | 664.40µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 921.41µs |  |  | 466.82µs | 1.199ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.584ms |  |  | 3.529ms | 7.837ms | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 185.26µs |  |  | 138.60µs | 264.07µs | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.693ms |  |  | 1.261ms | 2.270ms | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 848.53µs |  |  | 641.36µs | 1.137ms | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 210.23µs |  |  | 172.02µs | 312.70µs | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.843ms |  |  | 1.508ms | 2.579ms | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 956.80µs |  |  | 767.16µs | 1.307ms | 3 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 278.48µs |  |  | 178.63µs | 349.09µs | 3 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 17.412ms |  |  | 13.818ms | 27.704ms | 3 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 697.667ms |  |  | 374.892ms | 697.667ms | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 154.74µs |  |  | 129.80µs | 239.15µs | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.245ms |  |  | 1.087ms | 1.873ms | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 661.30µs |  |  | 540.35µs | 954.06µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 163.71µs |  |  | 101.09µs | 214.26µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 754.87µs |  |  | 478.58µs | 983.96µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 175.78µs |  |  | 110.99µs | 233.97µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 794.20µs |  |  | 500.02µs | 1.024ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.689ms |  |  | 1.930ms | 3.868ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.738ms |  |  | 1.940ms | 3.822ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.667ms |  |  | 1.882ms | 3.803ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.572ms |  |  | 1.769ms | 3.809ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.742ms |  |  | 1.146ms | 2.335ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.478ms |  |  | 1.800ms | 3.358ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.385ms |  |  | 1.739ms | 3.440ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 174.38µs |  |  | 146.54µs | 272.52µs | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 99.13µs |  |  | 77.01µs | 149.91µs | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.218ms |  |  | 926.00µs | 1.760ms | 3 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.409ms |  |  | 929.88µs | 1.985ms | 3 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.513ms |  |  | 979.01µs | 2.139ms | 3 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 34.12µs |  |  | 27.41µs | 55.03µs | 3 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 37.01µs |  |  | 29.01µs | 55.45µs | 3 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 51.24µs |  |  | 39.86µs | 72.43µs | 3 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.156ms |  |  | 768.96µs | 1.567ms | 3 |

informational; points come from different runners of the same class, so read trends, not single deltas.
