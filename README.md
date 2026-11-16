## aui-perf nightly record

_4 points · 2026-11-13T12:30:39.442Z to 2026-11-16T13:01:14.462Z · latest runner: AMD EPYC 9V45 96-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 458.02µs |  |  | 429.43µs | 859.20µs | 4 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 673.05µs |  |  | 657.87µs | 1.224ms | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 30.22µs |  |  | 30.22µs | 56.85µs | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 353.92µs |  |  | 353.92µs | 641.80µs | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.538ms |  |  | 5.538ms | 10.043ms | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 149.33µs |  |  | 148.79µs | 282.52µs | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.366ms |  |  | 1.366ms | 2.529ms | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.521ms |  |  | 5.512ms | 9.900ms | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 5.45µs |  |  | 5.16µs | 9.71µs | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 46.00µs |  |  | 43.60µs | 85.87µs | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 179.62µs |  |  | 168.77µs | 347.11µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 49.83µs |  |  | 49.83µs | 142.84µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 24.17µs |  |  | 23.77µs | 81.67µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 26.16µs |  |  | 26.16µs | 82.76µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 146.37µs |  |  | 146.37µs | 319.38µs | 4 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 38.95µs |  |  | 38.17µs | 75.45µs | 4 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 380.46µs |  |  | 359.63µs | 688.91µs | 4 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 5.31µs |  |  | 5.14µs | 10.18µs | 4 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 44.58µs |  |  | 44.58µs | 84.63µs | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 370.81µs |  |  | 367.93µs | 758.23µs | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.311ms |  |  | 3.247ms | 6.014ms | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 13.049ms |  |  | 12.796ms | 23.817ms | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 194.21µs |  |  | 190.34µs | 352.26µs | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 1.875ms |  |  | 1.873ms | 3.310ms | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 7.402ms |  |  | 7.286ms | 13.073ms | 4 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 137.70µs |  |  | 136.31µs | 274.11µs | 4 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 786.83µs |  |  | 786.83µs | 1.989ms | 4 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 34.42µs |  |  | 33.04µs | 68.04µs | 4 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 355.48µs |  |  | 343.49µs | 689.14µs | 4 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 1.912ms |  |  | 1.834ms | 3.677ms | 4 |
| external-message-conversion › core: external message tool results › 100 matches | 39.30µs |  |  | 37.37µs | 81.72µs | 4 |
| external-message-conversion › core: external message tool results › 1000 matches | 400.85µs |  |  | 384.57µs | 819.69µs | 4 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.096ms |  |  | 1.989ms | 4.221ms | 4 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 21.12µs |  |  | 20.26µs | 41.87µs | 4 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 199.94µs |  |  | 190.52µs | 411.84µs | 4 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.072ms |  |  | 1.041ms | 2.218ms | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.14µs |  |  | 0.14µs | 0.28µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.25µs |  |  | 0.24µs | 0.46µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.46µs |  |  | 1.42µs | 2.41µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.36µs |  |  | 0.34µs | 0.66µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 1.75µs |  |  | 1.63µs | 3.56µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 15.66µs |  |  | 14.96µs | 32.26µs | 4 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 87.70µs |  |  | 85.39µs | 153.69µs | 4 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 444.27µs |  |  | 436.67µs | 889.09µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.430ms |  |  | 1.327ms | 2.871ms | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 101.94µs |  |  | 97.31µs | 212.68µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 1.879ms |  |  | 1.744ms | 3.724ms | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 263.91µs |  |  | 243.79µs | 514.91µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 368.62µs |  |  | 351.48µs | 725.76µs | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 4.075ms |  |  | 3.741ms | 7.522ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 455.00µs |  |  | 441.49µs | 947.41µs | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 10.781ms |  |  | 10.454ms | 25.040ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 1.831ms |  |  | 1.727ms | 3.716ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.395ms |  |  | 1.367ms | 2.813ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.511ms |  |  | 1.455ms | 3.236ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 1.678ms |  |  | 1.662ms | 3.470ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 11.640ms |  |  | 10.846ms | 22.745ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 12.773ms |  |  | 12.252ms | 23.466ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 731.11µs |  |  | 731.11µs | 1.502ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.415ms |  |  | 1.415ms | 3.117ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 5.393ms |  |  | 5.340ms | 10.063ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.133ms |  |  | 1.133ms | 1.236ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.181ms |  |  | 1.178ms | 1.970ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 2.913ms |  |  | 2.913ms | 4.752ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 181.39µs |  |  | 174.54µs | 326.73µs | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.494ms |  |  | 1.494ms | 2.747ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 147.269ms |  |  | 142.981ms | 302.495ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 7.458ms |  |  | 7.458ms | 12.929ms | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.23µs |  |  | 1.22µs | 2.26µs | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.48µs |  |  | 5.48µs | 9.58µs | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 17.16µs |  |  | 17.16µs | 41.57µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.56µs |  |  | 4.42µs | 6.43µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 12.72µs |  |  | 12.72µs | 21.16µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 44.69µs |  |  | 44.35µs | 63.04µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 175.57µs |  |  | 175.04µs | 267.10µs | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 3.190ms |  |  | 3.190ms | 6.967ms | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 21.294ms |  |  | 21.294ms | 46.723ms | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 314.206ms |  |  | 314.158ms | 503.513ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 237.14µs |  |  | 237.14µs | 668.60µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 414.42µs |  |  | 391.88µs | 921.48µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 2.249ms |  |  | 1.837ms | 4.067ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 267.93µs |  |  | 253.67µs | 641.78µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 644.66µs |  |  | 644.66µs | 1.531ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 6.138ms |  |  | 6.138ms | 13.918ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 213.24µs |  |  | 213.24µs | 588.52µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 453.32µs |  |  | 453.32µs | 1.182ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 4.142ms |  |  | 3.532ms | 7.756ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 131.11µs |  |  | 109.91µs | 330.19µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 240.41µs |  |  | 240.41µs | 557.66µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 1.788ms |  |  | 1.596ms | 3.512ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 8.55µs |  |  | 8.55µs | 22.69µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 18.08µs |  |  | 18.08µs | 41.60µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 140.04µs |  |  | 125.87µs | 271.30µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 241.57µs |  |  | 241.57µs | 664.40µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 448.90µs |  |  | 448.90µs | 1.199ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 3.496ms |  |  | 3.496ms | 7.837ms | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 137.02µs |  |  | 137.02µs | 264.07µs | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.250ms |  |  | 1.250ms | 2.270ms | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 634.86µs |  |  | 634.86µs | 1.137ms | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 168.40µs |  |  | 168.40µs | 312.70µs | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.478ms |  |  | 1.478ms | 2.579ms | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 755.79µs |  |  | 755.79µs | 1.307ms | 4 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 183.00µs |  |  | 178.63µs | 349.09µs | 4 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 13.466ms |  |  | 13.466ms | 27.704ms | 4 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 366.485ms |  |  | 366.485ms | 697.667ms | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 129.76µs |  |  | 129.76µs | 239.15µs | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.064ms |  |  | 1.064ms | 1.873ms | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 538.78µs |  |  | 538.78µs | 954.06µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 106.46µs |  |  | 101.09µs | 214.26µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 493.57µs |  |  | 478.58µs | 983.96µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 114.66µs |  |  | 110.99µs | 233.97µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 525.03µs |  |  | 500.02µs | 1.024ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 1.926ms |  |  | 1.926ms | 3.868ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 1.961ms |  |  | 1.940ms | 3.822ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 1.862ms |  |  | 1.862ms | 3.803ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 1.801ms |  |  | 1.769ms | 3.809ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.162ms |  |  | 1.146ms | 2.335ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 1.817ms |  |  | 1.800ms | 3.358ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 1.753ms |  |  | 1.739ms | 3.440ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 143.94µs |  |  | 143.94µs | 272.52µs | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 78.59µs |  |  | 77.01µs | 149.91µs | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 952.75µs |  |  | 926.00µs | 1.760ms | 4 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 977.28µs |  |  | 929.88µs | 1.985ms | 4 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.008ms |  |  | 979.01µs | 2.139ms | 4 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 27.41µs |  |  | 27.41µs | 55.03µs | 4 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 28.76µs |  |  | 28.76µs | 55.45µs | 4 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 39.50µs |  |  | 39.50µs | 72.43µs | 4 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 811.09µs |  |  | 768.96µs | 1.567ms | 4 |

informational; points come from different runners of the same class, so read trends, not single deltas.
