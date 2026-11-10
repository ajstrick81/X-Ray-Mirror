# X-Ray Mirror

A copy of the creator’s single-file X-Ray Mirror app, published with the permission granted by u/Sourcecode12 in the original Reddit discussion. The application HTML and embedded 3D anatomy mesh are taken from the creator’s public GitHub repository; this hosted copy adds attribution and a short external-asset notice.

- Creator’s live project: [masterofvfx2070.github.io/xray-mirror](https://masterofvfx2070.github.io/xray-mirror/)
- Creator’s source repository: [MasterOfVFX2070/xray-mirror](https://github.com/MasterOfVFX2070/xray-mirror)
- Original Reddit post and permission: [r/ClaudeAI post by u/Sourcecode12](https://www.reddit.com/r/ClaudeAI/comments/1xstews/i_built_a_webcam_xray_mirror_with_claude_fable_52/)

## Camera and network behavior

The HTML requests camera access with `getUserMedia` and performs face and hand tracking in the browser. Static inspection found no camera-frame upload code. The browser does request Three.js, MediaPipe, WASM runtime files, and tracker models from jsDelivr and Google Storage; those hosts receive normal asset requests.

The app credits the anatomy models to BodyParts3D, © The Database Center for Life Science, CC Attribution-Share Alike 2.1 Japan. The creator notes that the models were simplified and re-aligned.
