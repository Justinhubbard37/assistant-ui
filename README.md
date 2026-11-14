## aui-perf nightly record

_2 points · 2026-11-13T12:30:39.442Z to 2026-11-14T11:43:54.739Z · latest runner: AMD EPYC 9V45 96-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 429.43µs |  |  | 429.43µs | 859.20µs | 2 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 657.87µs |  |  | 657.87µs | 1.224ms | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 30.56µs |  |  | 30.56µs | 56.85µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 361.89µs |  |  | 361.89µs | 641.80µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.568ms |  |  | 5.568ms | 10.043ms | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 148.79µs |  |  | 148.79µs | 282.52µs | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.370ms |  |  | 1.370ms | 2.529ms | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.512ms |  |  | 5.512ms | 9.900ms | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 5.16µs |  |  | 5.16µs | 9.71µs | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 43.60µs |  |  | 43.60µs | 85.87µs | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 168.77µs |  |  | 168.77µs | 347.11µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 50.90µs |  |  | 50.90µs | 142.84µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 23.77µs |  |  | 23.77µs | 81.67µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 26.20µs |  |  | 26.20µs | 82.76µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 149.36µs |  |  | 149.36µs | 319.38µs | 2 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 38.17µs |  |  | 38.17µs | 75.45µs | 2 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 359.63µs |  |  | 359.63µs | 688.91µs | 2 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 5.14µs |  |  | 5.14µs | 10.18µs | 2 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 45.08µs |  |  | 45.08µs | 84.63µs | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 367.93µs |  |  | 367.93µs | 758.23µs | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.247ms |  |  | 3.247ms | 6.014ms | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 12.796ms |  |  | 12.796ms | 23.817ms | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 190.34µs |  |  | 190.34µs | 352.26µs | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 1.873ms |  |  | 1.873ms | 3.310ms | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 7.286ms |  |  | 7.286ms | 13.073ms | 2 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 136.31µs |  |  | 136.31µs | 274.11µs | 2 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 794.22µs |  |  | 794.22µs | 1.989ms | 2 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 33.04µs |  |  | 33.04µs | 68.04µs | 2 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 343.49µs |  |  | 343.49µs | 689.14µs | 2 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 1.834ms |  |  | 1.834ms | 3.677ms | 2 |
| external-message-conversion › core: external message tool results › 100 matches | 37.37µs |  |  | 37.37µs | 81.72µs | 2 |
| external-message-conversion › core: external message tool results › 1000 matches | 384.57µs |  |  | 384.57µs | 819.69µs | 2 |
| external-message-conversion › core: external message tool results › 5000 matches | 1.989ms |  |  | 1.989ms | 4.221ms | 2 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 20.26µs |  |  | 20.26µs | 41.87µs | 2 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 190.52µs |  |  | 190.52µs | 411.84µs | 2 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.041ms |  |  | 1.041ms | 2.218ms | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.14µs |  |  | 0.14µs | 0.28µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.24µs |  |  | 0.24µs | 0.46µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.42µs |  |  | 1.42µs | 2.41µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.34µs |  |  | 0.34µs | 0.66µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 1.63µs |  |  | 1.63µs | 3.56µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 14.96µs |  |  | 14.96µs | 32.26µs | 2 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 85.39µs |  |  | 85.39µs | 153.69µs | 2 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 436.67µs |  |  | 436.67µs | 889.09µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.327ms |  |  | 1.327ms | 2.871ms | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 97.31µs |  |  | 97.31µs | 212.68µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 1.744ms |  |  | 1.744ms | 3.724ms | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 243.79µs |  |  | 243.79µs | 514.91µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 351.48µs |  |  | 351.48µs | 725.76µs | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 3.741ms |  |  | 3.741ms | 7.522ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 441.49µs |  |  | 441.49µs | 947.41µs | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 10.454ms |  |  | 10.454ms | 25.040ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 1.727ms |  |  | 1.727ms | 3.716ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.367ms |  |  | 1.367ms | 2.813ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.455ms |  |  | 1.455ms | 3.236ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 1.662ms |  |  | 1.662ms | 3.470ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 10.846ms |  |  | 10.846ms | 22.745ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 12.252ms |  |  | 12.252ms | 23.466ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 758.93µs |  |  | 758.93µs | 1.502ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.446ms |  |  | 1.446ms | 3.117ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 5.340ms |  |  | 5.340ms | 10.063ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.145ms |  |  | 1.145ms | 1.188ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.178ms |  |  | 1.178ms | 1.970ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 2.946ms |  |  | 2.946ms | 4.752ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 174.54µs |  |  | 174.54µs | 326.73µs | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.543ms |  |  | 1.543ms | 2.747ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 142.981ms |  |  | 142.981ms | 302.495ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 7.502ms |  |  | 7.502ms | 12.929ms | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.22µs |  |  | 1.22µs | 2.26µs | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.66µs |  |  | 5.66µs | 9.58µs | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 17.49µs |  |  | 17.49µs | 41.57µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.42µs |  |  | 4.42µs | 6.43µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 12.94µs |  |  | 12.94µs | 21.16µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 44.35µs |  |  | 44.35µs | 63.04µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 175.04µs |  |  | 175.04µs | 267.10µs | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 3.376ms |  |  | 3.376ms | 6.967ms | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 23.023ms |  |  | 23.023ms | 46.723ms | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 322.203ms |  |  | 322.203ms | 503.513ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 240.55µs |  |  | 240.55µs | 668.60µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 391.88µs |  |  | 391.88µs | 921.48µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 1.837ms |  |  | 1.837ms | 4.067ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 253.67µs |  |  | 253.67µs | 641.78µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 734.91µs |  |  | 734.91µs | 1.531ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 6.328ms |  |  | 6.328ms | 13.918ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 230.48µs |  |  | 230.48µs | 588.52µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 495.91µs |  |  | 495.91µs | 1.182ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 3.532ms |  |  | 3.532ms | 7.756ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 109.91µs |  |  | 109.91µs | 330.19µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 243.26µs |  |  | 243.26µs | 557.66µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 1.596ms |  |  | 1.596ms | 3.512ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 8.63µs |  |  | 8.63µs | 22.69µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 18.83µs |  |  | 18.83µs | 41.60µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 125.87µs |  |  | 125.87µs | 271.30µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 261.56µs |  |  | 261.56µs | 664.40µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 466.82µs |  |  | 466.82µs | 1.199ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 3.529ms |  |  | 3.529ms | 7.837ms | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 138.60µs |  |  | 138.60µs | 264.07µs | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.261ms |  |  | 1.261ms | 2.270ms | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 641.36µs |  |  | 641.36µs | 1.137ms | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 172.02µs |  |  | 172.02µs | 312.70µs | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.508ms |  |  | 1.508ms | 2.579ms | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 767.16µs |  |  | 767.16µs | 1.307ms | 2 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 178.63µs |  |  | 178.63µs | 349.09µs | 2 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 13.818ms |  |  | 13.818ms | 27.704ms | 2 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 374.892ms |  |  | 374.892ms | 692.821ms | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 129.80µs |  |  | 129.80µs | 239.15µs | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.087ms |  |  | 1.087ms | 1.873ms | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 540.35µs |  |  | 540.35µs | 954.06µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 101.09µs |  |  | 101.09µs | 214.26µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 478.58µs |  |  | 478.58µs | 983.96µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 110.99µs |  |  | 110.99µs | 233.97µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 500.02µs |  |  | 500.02µs | 1.024ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 1.930ms |  |  | 1.930ms | 3.868ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 1.940ms |  |  | 1.940ms | 3.822ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 1.882ms |  |  | 1.882ms | 3.803ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 1.769ms |  |  | 1.769ms | 3.809ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.146ms |  |  | 1.146ms | 2.335ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 1.800ms |  |  | 1.800ms | 3.358ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 1.739ms |  |  | 1.739ms | 3.440ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 146.54µs |  |  | 146.54µs | 272.52µs | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 77.01µs |  |  | 77.01µs | 149.91µs | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 926.00µs |  |  | 926.00µs | 1.760ms | 2 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 929.88µs |  |  | 929.88µs | 1.985ms | 2 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 979.01µs |  |  | 979.01µs | 2.139ms | 2 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 27.41µs |  |  | 27.41µs | 55.03µs | 2 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 29.01µs |  |  | 29.01µs | 55.45µs | 2 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 39.86µs |  |  | 39.86µs | 72.43µs | 2 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 768.96µs |  |  | 768.96µs | 1.567ms | 2 |

informational; points come from different runners of the same class, so read trends, not single deltas.
