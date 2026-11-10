# X-Ray Mirror

A GitHub Pages copy of the single-file X-Ray Mirror by u/Sourcecode12, shared with the creator’s permission. The original application code and embedded 3D anatomy mesh are preserved; this copy adds a courtesy attribution, a link to the original Reddit post, and a note about external runtime asset requests.

- [Try the original Reddit post and download](https://www.reddit.com/r/ClaudeAI/comments/1xstews/i_built_a_webcam_xray_mirror_with_claude_fable_52/)
- [Creator: u/Sourcecode12](https://www.reddit.com/user/Sourcecode12/)

## Camera and network behavior

The HTML requests camera access with `getUserMedia` and performs face and hand tracking in the browser. Static inspection found no camera-frame upload or telemetry code. The browser does request Three.js, MediaPipe, WASM runtime files, and tracker model files from jsDelivr and Google Storage. Those hosts therefore receive normal asset requests. A camera-enabled secure origin is required; GitHub Pages provides HTTPS.

The anatomy models are attributed in the app to BodyParts3D, © The Database Center for Life Science, CC BY-SA 2.1 Japan, with models simplified and re-aligned by the creator.
