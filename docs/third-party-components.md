# Models, Datasets, APIs, and Third-Party Components

## 1. AI Models

### MediaPipe Pose
Purpose: Body landmark estimation from camera frames, if the library and its model assets are configured in the current application.

### Generative Virtual Try-On Models
No generative garment-replacement model is documented as part of the current prototype unless one has been separately integrated.

## 2. Datasets

The application uses live camera input and the clothing graphics included with the project.

No separate machine-learning training dataset is claimed for the current implementation.

## 3. APIs

### Browser MediaDevices API
Purpose: Access the user's camera through browser permissions, if the application uses `getUserMedia()`.

### HTML Canvas API
Purpose: Draw clothing overlays and compose visual output.

## 4. Third-Party Libraries

- MediaPipe Pose, if used in the source code.
- External JavaScript libraries loaded from a CDN, if configured.
- Any additional dependencies discovered in the application source.

## 5. Dependency Details

Before submitting, record the exact package name, version, source URL, and license for each external library and model asset.

Do not guess versions or list libraries that are not used by the application.

## 6. Privacy and Security

- Do not commit API keys or credentials.
- Verify whether camera frames are processed locally or transmitted elsewhere before making privacy claims.
- Review the licenses of third-party libraries and clothing assets before redistribution.