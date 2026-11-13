## aui-perf nightly record

_1 points · 2026-11-13T12:30:39.442Z to 2026-11-13T12:30:39.442Z · latest runner: AMD EPYC 7763 64-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 859.20µs |  |  | 859.20µs | 859.20µs | 1 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.224ms |  |  | 1.224ms | 1.224ms | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 56.85µs |  |  | 56.85µs | 56.85µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 641.80µs |  |  | 641.80µs | 641.80µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 10.043ms |  |  | 10.043ms | 10.043ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 282.52µs |  |  | 282.52µs | 282.52µs | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.529ms |  |  | 2.529ms | 2.529ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 9.900ms |  |  | 9.900ms | 9.900ms | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 9.71µs |  |  | 9.71µs | 9.71µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 85.87µs |  |  | 85.87µs | 85.87µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 347.11µs |  |  | 347.11µs | 347.11µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 142.84µs |  |  | 142.84µs | 142.84µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 81.67µs |  |  | 81.67µs | 81.67µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 82.76µs |  |  | 82.76µs | 82.76µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 319.38µs |  |  | 319.38µs | 319.38µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 75.45µs |  |  | 75.45µs | 75.45µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 688.91µs |  |  | 688.91µs | 688.91µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 10.18µs |  |  | 10.18µs | 10.18µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 84.63µs |  |  | 84.63µs | 84.63µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 758.23µs |  |  | 758.23µs | 758.23µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 6.014ms |  |  | 6.014ms | 6.014ms | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 23.817ms |  |  | 23.817ms | 23.817ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 352.26µs |  |  | 352.26µs | 352.26µs | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 3.310ms |  |  | 3.310ms | 3.310ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 13.073ms |  |  | 13.073ms | 13.073ms | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 274.11µs |  |  | 274.11µs | 274.11µs | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.989ms |  |  | 1.989ms | 1.989ms | 1 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 68.04µs |  |  | 68.04µs | 68.04µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 689.14µs |  |  | 689.14µs | 689.14µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 3.677ms |  |  | 3.677ms | 3.677ms | 1 |
| external-message-conversion › core: external message tool results › 100 matches | 81.72µs |  |  | 81.72µs | 81.72µs | 1 |
| external-message-conversion › core: external message tool results › 1000 matches | 819.69µs |  |  | 819.69µs | 819.69µs | 1 |
| external-message-conversion › core: external message tool results › 5000 matches | 4.221ms |  |  | 4.221ms | 4.221ms | 1 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 41.87µs |  |  | 41.87µs | 41.87µs | 1 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 411.84µs |  |  | 411.84µs | 411.84µs | 1 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 2.218ms |  |  | 2.218ms | 2.218ms | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.28µs |  |  | 0.28µs | 0.28µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.46µs |  |  | 0.46µs | 0.46µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.41µs |  |  | 2.41µs | 2.41µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.66µs |  |  | 0.66µs | 0.66µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 3.56µs |  |  | 3.56µs | 3.56µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 32.26µs |  |  | 32.26µs | 32.26µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 153.69µs |  |  | 153.69µs | 153.69µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 889.09µs |  |  | 889.09µs | 889.09µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.871ms |  |  | 2.871ms | 2.871ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 212.68µs |  |  | 212.68µs | 212.68µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 3.724ms |  |  | 3.724ms | 3.724ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 514.91µs |  |  | 514.91µs | 514.91µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 725.76µs |  |  | 725.76µs | 725.76µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 7.522ms |  |  | 7.522ms | 7.522ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 947.41µs |  |  | 947.41µs | 947.41µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 25.040ms |  |  | 25.040ms | 25.040ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 3.716ms |  |  | 3.716ms | 3.716ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 2.813ms |  |  | 2.813ms | 2.813ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 3.236ms |  |  | 3.236ms | 3.236ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 3.470ms |  |  | 3.470ms | 3.470ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 22.745ms |  |  | 22.745ms | 22.745ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 23.466ms |  |  | 23.466ms | 23.466ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.502ms |  |  | 1.502ms | 1.502ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 3.117ms |  |  | 3.117ms | 3.117ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 10.063ms |  |  | 10.063ms | 10.063ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.188ms |  |  | 1.188ms | 1.188ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.970ms |  |  | 1.970ms | 1.970ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.752ms |  |  | 4.752ms | 4.752ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 326.73µs |  |  | 326.73µs | 326.73µs | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.747ms |  |  | 2.747ms | 2.747ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 302.495ms |  |  | 302.495ms | 302.495ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 12.929ms |  |  | 12.929ms | 12.929ms | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 2.26µs |  |  | 2.26µs | 2.26µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 9.58µs |  |  | 9.58µs | 9.58µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 41.57µs |  |  | 41.57µs | 41.57µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 6.43µs |  |  | 6.43µs | 6.43µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 21.16µs |  |  | 21.16µs | 21.16µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 63.04µs |  |  | 63.04µs | 63.04µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 267.10µs |  |  | 267.10µs | 267.10µs | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 6.967ms |  |  | 6.967ms | 6.967ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 46.723ms |  |  | 46.723ms | 46.723ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 503.513ms |  |  | 503.513ms | 503.513ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 668.60µs |  |  | 668.60µs | 668.60µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 921.48µs |  |  | 921.48µs | 921.48µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 4.067ms |  |  | 4.067ms | 4.067ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 641.78µs |  |  | 641.78µs | 641.78µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.531ms |  |  | 1.531ms | 1.531ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 13.918ms |  |  | 13.918ms | 13.918ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 588.52µs |  |  | 588.52µs | 588.52µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 1.182ms |  |  | 1.182ms | 1.182ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 7.756ms |  |  | 7.756ms | 7.756ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 330.19µs |  |  | 330.19µs | 330.19µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 557.66µs |  |  | 557.66µs | 557.66µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 3.512ms |  |  | 3.512ms | 3.512ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 22.69µs |  |  | 22.69µs | 22.69µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 41.60µs |  |  | 41.60µs | 41.60µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 271.30µs |  |  | 271.30µs | 271.30µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 664.40µs |  |  | 664.40µs | 664.40µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 1.199ms |  |  | 1.199ms | 1.199ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 7.837ms |  |  | 7.837ms | 7.837ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 264.07µs |  |  | 264.07µs | 264.07µs | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 2.270ms |  |  | 2.270ms | 2.270ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 1.137ms |  |  | 1.137ms | 1.137ms | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 312.70µs |  |  | 312.70µs | 312.70µs | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.579ms |  |  | 2.579ms | 2.579ms | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.307ms |  |  | 1.307ms | 1.307ms | 1 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 349.09µs |  |  | 349.09µs | 349.09µs | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 27.704ms |  |  | 27.704ms | 27.704ms | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 692.821ms |  |  | 692.821ms | 692.821ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 239.15µs |  |  | 239.15µs | 239.15µs | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.873ms |  |  | 1.873ms | 1.873ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 954.06µs |  |  | 954.06µs | 954.06µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 214.26µs |  |  | 214.26µs | 214.26µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 983.96µs |  |  | 983.96µs | 983.96µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 233.97µs |  |  | 233.97µs | 233.97µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 1.024ms |  |  | 1.024ms | 1.024ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 3.868ms |  |  | 3.868ms | 3.868ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 3.822ms |  |  | 3.822ms | 3.822ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 3.803ms |  |  | 3.803ms | 3.803ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 3.809ms |  |  | 3.809ms | 3.809ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 2.335ms |  |  | 2.335ms | 2.335ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 3.358ms |  |  | 3.358ms | 3.358ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 3.440ms |  |  | 3.440ms | 3.440ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 272.52µs |  |  | 272.52µs | 272.52µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 149.91µs |  |  | 149.91µs | 149.91µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.760ms |  |  | 1.760ms | 1.760ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.985ms |  |  | 1.985ms | 1.985ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 2.139ms |  |  | 2.139ms | 2.139ms | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 55.03µs |  |  | 55.03µs | 55.03µs | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 55.45µs |  |  | 55.45µs | 55.45µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 72.43µs |  |  | 72.43µs | 72.43µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.567ms |  |  | 1.567ms | 1.567ms | 1 |

informational; points come from different runners of the same class, so read trends, not single deltas.
