---
-api-type: winrt class
---
 [Visual](visual.md) – base object, the majority of the properties are here, and inherited by the other Visual objects.
 [ContainerVisual](containervisual.md) – derives from [Visual](visual.md), and adds the ability to create children.
 [SpriteVisual](spritevisual.md) – derives from [ContainerVisual](containervisual.md), and contains content in the form of images, effects, and swapchains.
 [Compositor](compositor.md) – manages the relationship between an application and the system compositor process.
 [KeyFrameAnimation](keyframeanimation.md): Time-based animations with two or more key frames. These frames are markers, allowing developers to define what the animated value should be at the specified time. Animations can additionally be fine-tuned by specifying how the animation interpolates (blends) the values between key frames. [KeyFrameAnimation](keyframeanimation.md) has many subclasses each supporting a different type of key frame value.
 [ExpressionAnimation](expressionanimation.md): Animations that use a mathematical expression to specify how the animated value should be calculated each frame. The expressions can reference properties from composition objects. [ExpressionAnimation](expressionanimation.md) s are not time-based and are processed each frame (if necessary).