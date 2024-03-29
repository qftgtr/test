# Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`class `[`NRKernal::NRAnchor`](#class_n_r_kernal_1_1_n_r_anchor) | Update the transform of a trackable.
`class `[`NRKernal::NRCameraCapture`](#class_n_r_kernal_1_1_n_r_camera_capture) | Manage the image update of rgb camera.
`class `[`NRKernal::NRFrame`](#class_n_r_kernal_1_1_n_r_frame) | Holds information about NR Device's pose in the world coordinate, trackables, etc..
`class `[`NRKernal::NRInput`](#class_n_r_kernal_1_1_n_r_input) | The main class to handle controller related things, such as to get controller states, update controller states.
`class `[`NRKernal::NRRenderer`](#class_n_r_kernal_1_1_n_r_renderer) | NRNativeRender oprate rendering-related things, provides the feature of ATW and low latency.
`class `[`NRKernal::NRRgbCamera`](#class_n_r_kernal_1_1_n_r_rgb_camera) | Manage the life cycle of the entire rgbcamera.
`class `[`NRKernal::NRSessionBehaviour`](#class_n_r_kernal_1_1_n_r_session_behaviour) | Oprate AR system state and handles the session lifecycle for application layer.
`class `[`NRKernal::NRSessionConfig`](#class_n_r_kernal_1_1_n_r_session_config) | A configuration used to track the world.
`class `[`NRKernal::NRSessionManager`](#class_n_r_kernal_1_1_n_r_session_manager) | Manages AR system state and handles the session lifecycle.
`class `[`NRKernal::NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable) | A Trackable in the real world detected by NRInternel.
`class `[`NRKernal::NRTrackableBehaviour`](#class_n_r_kernal_1_1_n_r_trackable_behaviour) | Base classes for all trackable monobehaviour objects.
`class `[`NRKernal::NRTrackableImage`](#class_n_r_kernal_1_1_n_r_trackable_image) | A trackable image in the real world detected by NRInternel.
`class `[`NRKernal::NRTrackableManager`](#class_n_r_kernal_1_1_n_r_trackable_manager) | Manages AR system state and handles the session lifecycle.
`class `[`NRKernal::NRTrackablePlane`](#class_n_r_kernal_1_1_n_r_trackable_plane) | A plane in the real world detected by NRInternel.
`class `[`NRKernal::NRTrackingImageDatabase`](#class_n_r_kernal_1_1_n_r_tracking_image_database) | A database storing a list of images to be detected and tracked by NRSDK.
`class `[`NRKernal::NRVersionInfo`](#class_n_r_kernal_1_1_n_r_version_info) | Holds information about Nreal SDK version info.
`struct `[`NRKernal::NRTrackingImageDatabaseEntry`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry) | Hold the total infomation of a image data base item.

# class `NRKernal::NRAnchor` 

```
class NRKernal::NRAnchor
  : public MonoBehaviour
```  

Update the transform of a trackable.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public `[`NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable)` `[`Trackable`](#class_n_r_kernal_1_1_n_r_anchor_1a4857530b80ac3d063d8589e97610b21e) | 

## Members

#### `public `[`NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable)` `[`Trackable`](#class_n_r_kernal_1_1_n_r_anchor_1a4857530b80ac3d063d8589e97610b21e) 

# class `NRKernal::NRCameraCapture` 

```
class NRKernal::NRCameraCapture
  : public MonoBehaviour
```  

Manage the image update of rgb camera.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} CameraImageFormat `[`ImageFormat`](#class_n_r_kernal_1_1_n_r_camera_capture_1a31c9bdac11c2175fb73b8e69b6e6262a) | Image format of rgb camera.
`{property} int `[`FrameCount`](#class_n_r_kernal_1_1_n_r_camera_capture_1a0fa6048425ba83a9fcbf3581df531434) | Current frame count of rgb camera.
`{property} IntPtr `[`TexturePtr`](#class_n_r_kernal_1_1_n_r_camera_capture_1a6c31d660f1730cee35839e799b0f499f) | Texture ptr of rgb camera.
`{property} NativeResolution `[`Resolution`](#class_n_r_kernal_1_1_n_r_camera_capture_1a4356a4144d7be348cf4b7603b16bea5f) | Resolution of rgb camera.
`{property} int `[`UpdateFrameRate`](#class_n_r_kernal_1_1_n_r_camera_capture_1a21a55b1f4aaa13d508b224a52bfd2ac2) | 
`public NRRgbCamera.CaptureEvent `[`OnFirstFramReady`](#class_n_r_kernal_1_1_n_r_camera_capture_1a11742f5135879d773549d6bf81617c3f) | 
`public NRRgbCamera.CaptureErrorEvent `[`OnError`](#class_n_r_kernal_1_1_n_r_camera_capture_1a23eaa223864ae62feb08e31054260d41) | 
`public Texture2D `[`Texture`](#class_n_r_kernal_1_1_n_r_camera_capture_1abcd34b994621385db38366ad297581b6) | Texture2D of rgb camera.
`public inline void `[`Play`](#class_n_r_kernal_1_1_n_r_camera_capture_1a6d584c1d0bb359b0f03a51909724b1c4)`()` | Start to play rgb camera.
`public inline void `[`Stop`](#class_n_r_kernal_1_1_n_r_camera_capture_1aa03fa1874172c27d7e6212a2c0adccda)`()` | Stop rgb camera.
`public inline void `[`Release`](#class_n_r_kernal_1_1_n_r_camera_capture_1af89e10329b74874d24a41b41acfe2dc3)`()` | Release to play rgb camera.

## Members

#### `{property} CameraImageFormat `[`ImageFormat`](#class_n_r_kernal_1_1_n_r_camera_capture_1a31c9bdac11c2175fb73b8e69b6e6262a) 

Image format of rgb camera.

#### `{property} int `[`FrameCount`](#class_n_r_kernal_1_1_n_r_camera_capture_1a0fa6048425ba83a9fcbf3581df531434) 

Current frame count of rgb camera.

#### `{property} IntPtr `[`TexturePtr`](#class_n_r_kernal_1_1_n_r_camera_capture_1a6c31d660f1730cee35839e799b0f499f) 

Texture ptr of rgb camera.

#### `{property} NativeResolution `[`Resolution`](#class_n_r_kernal_1_1_n_r_camera_capture_1a4356a4144d7be348cf4b7603b16bea5f) 

Resolution of rgb camera.

#### `{property} int `[`UpdateFrameRate`](#class_n_r_kernal_1_1_n_r_camera_capture_1a21a55b1f4aaa13d508b224a52bfd2ac2) 

#### `public NRRgbCamera.CaptureEvent `[`OnFirstFramReady`](#class_n_r_kernal_1_1_n_r_camera_capture_1a11742f5135879d773549d6bf81617c3f) 

#### `public NRRgbCamera.CaptureErrorEvent `[`OnError`](#class_n_r_kernal_1_1_n_r_camera_capture_1a23eaa223864ae62feb08e31054260d41) 

#### `public Texture2D `[`Texture`](#class_n_r_kernal_1_1_n_r_camera_capture_1abcd34b994621385db38366ad297581b6) 

Texture2D of rgb camera.

#### `public inline void `[`Play`](#class_n_r_kernal_1_1_n_r_camera_capture_1a6d584c1d0bb359b0f03a51909724b1c4)`()` 

Start to play rgb camera.

#### `public inline void `[`Stop`](#class_n_r_kernal_1_1_n_r_camera_capture_1aa03fa1874172c27d7e6212a2c0adccda)`()` 

Stop rgb camera.

#### `public inline void `[`Release`](#class_n_r_kernal_1_1_n_r_camera_capture_1af89e10329b74874d24a41b41acfe2dc3)`()` 

Release to play rgb camera.

# class `NRKernal::NRFrame` 

Holds information about NR Device's pose in the world coordinate, trackables, etc..

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} TrackingState `[`TrackingStatus`](#class_n_r_kernal_1_1_n_r_frame_1a67dfb67709f00175f8046089970aec17) | Get the tracking state of HMD.
`{property} LostTrackingReason `[`LostTrackingReason`](#class_n_r_kernal_1_1_n_r_frame_1ac882fece9cb92947e23e1c2b908d166e) | Get the lost tracking reason of HMD.
`{property} Pose `[`HeadPose`](#class_n_r_kernal_1_1_n_r_frame_1ac3096f609a646a3d754bd87de25fe989) | Get the pose of device in unity world coordinate.
`{property} Pose `[`CenterEyePose`](#class_n_r_kernal_1_1_n_r_frame_1ad3788dd75a7ef53eb15d5c25c206149b) | Get the pose of center camera between left eye and right eye.
`{property} EyePosData `[`EyePosFromHead`](#class_n_r_kernal_1_1_n_r_frame_1a3c7a080d9eb1fc5be603cc205944f0af) | Get the offset position between eye and head.

## Members

#### `{property} TrackingState `[`TrackingStatus`](#class_n_r_kernal_1_1_n_r_frame_1a67dfb67709f00175f8046089970aec17) 

Get the tracking state of HMD.

#### `{property} LostTrackingReason `[`LostTrackingReason`](#class_n_r_kernal_1_1_n_r_frame_1ac882fece9cb92947e23e1c2b908d166e) 

Get the lost tracking reason of HMD.

#### `{property} Pose `[`HeadPose`](#class_n_r_kernal_1_1_n_r_frame_1ac3096f609a646a3d754bd87de25fe989) 

Get the pose of device in unity world coordinate.

#### Returns
Pose of device.

#### `{property} Pose `[`CenterEyePose`](#class_n_r_kernal_1_1_n_r_frame_1ad3788dd75a7ef53eb15d5c25c206149b) 

Get the pose of center camera between left eye and right eye.

#### `{property} EyePosData `[`EyePosFromHead`](#class_n_r_kernal_1_1_n_r_frame_1a3c7a080d9eb1fc5be603cc205944f0af) 

Get the offset position between eye and head.

# class `NRKernal::NRInput` 

```
class NRKernal::NRInput
  : public MonoBehaviour
```  

The main class to handle controller related things, such as to get controller states, update controller states.

Through this class, application would create a controllerProvider which could be custom, then the controllerProvider iteself would define how to update the controller states, so that every frame [NRInput](#class_n_r_kernal_1_1_n_r_input) could get the right states. There are max two states for one controllerProvider.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} `[`NRInput`](#class_n_r_kernal_1_1_n_r_input)` `[`Instance`](#class_n_r_kernal_1_1_n_r_input_1adc0907cdc783e79c341370c24382b86c) | 
`{property} bool `[`ReticleVisualActive`](#class_n_r_kernal_1_1_n_r_input_1af296428d8d111d96d706828be0cff963) | Determine whether to show reticle visuals, could be get and set at runtime.
`{property} bool `[`LaserVisualActive`](#class_n_r_kernal_1_1_n_r_input_1ab548c8084aa7d17cff1813b27182761e) | Determine whether to show laser visuals, could be get and set at runtime.
`{property} bool `[`ControllerVisualActive`](#class_n_r_kernal_1_1_n_r_input_1a62693b01aca0023f00fa80869665f936) | Determine whether to show controller visuals, could be get and set at runtime.
`{property} bool `[`HapticVibrationEnabled`](#class_n_r_kernal_1_1_n_r_input_1ab9a5f2f45176084475648300642a8740) | Determine whether enable haptic vibration.
`{property} ControllerAnchorsHelper `[`AnchorsHelper`](#class_n_r_kernal_1_1_n_r_input_1a98b0c518f55b5182304e37e819f8a8b9) | It's a helper to get controller anchors which are frequently used.
`{property} `[`ControllerHandEnum`](#namespace_n_r_kernal_1a07ed61c4e0d1b9780a26dce08fe6e3ae)` `[`DomainHand`](#class_n_r_kernal_1_1_n_r_input_1aafc4500538b90bdedc26c0cf91e772e6) | Get the current enumeration of handedness.
`{property} `[`RaycastModeEnum`](#namespace_n_r_kernal_1ae5741edcbe09473334e44c714bcb8c17)` `[`RaycastMode`](#class_n_r_kernal_1_1_n_r_input_1ad9e00319cf4326e3ad9e5a23f56fd1a9) | Determine which raycast mode to use.
`{property} Transform `[`CameraCenter`](#class_n_r_kernal_1_1_n_r_input_1a706e9b4b0c14626bdc72682c9bcb6a3f) | Get the transform of the camera which controllers are following.
`public const int `[`MAX_CONTROLLER_STATE_COUNT`](#class_n_r_kernal_1_1_n_r_input_1aec18a837233e50bb2a0ba96798010b21) | Max count of controllerstates supported per frame.

## Members

#### `{property} `[`NRInput`](#class_n_r_kernal_1_1_n_r_input)` `[`Instance`](#class_n_r_kernal_1_1_n_r_input_1adc0907cdc783e79c341370c24382b86c) 

#### `{property} bool `[`ReticleVisualActive`](#class_n_r_kernal_1_1_n_r_input_1af296428d8d111d96d706828be0cff963) 

Determine whether to show reticle visuals, could be get and set at runtime.

#### `{property} bool `[`LaserVisualActive`](#class_n_r_kernal_1_1_n_r_input_1ab548c8084aa7d17cff1813b27182761e) 

Determine whether to show laser visuals, could be get and set at runtime.

#### `{property} bool `[`ControllerVisualActive`](#class_n_r_kernal_1_1_n_r_input_1a62693b01aca0023f00fa80869665f936) 

Determine whether to show controller visuals, could be get and set at runtime.

#### `{property} bool `[`HapticVibrationEnabled`](#class_n_r_kernal_1_1_n_r_input_1ab9a5f2f45176084475648300642a8740) 

Determine whether enable haptic vibration.

#### `{property} ControllerAnchorsHelper `[`AnchorsHelper`](#class_n_r_kernal_1_1_n_r_input_1a98b0c518f55b5182304e37e819f8a8b9) 

It's a helper to get controller anchors which are frequently used.

#### `{property} `[`ControllerHandEnum`](#namespace_n_r_kernal_1a07ed61c4e0d1b9780a26dce08fe6e3ae)` `[`DomainHand`](#class_n_r_kernal_1_1_n_r_input_1aafc4500538b90bdedc26c0cf91e772e6) 

Get the current enumeration of handedness.

#### `{property} `[`RaycastModeEnum`](#namespace_n_r_kernal_1ae5741edcbe09473334e44c714bcb8c17)` `[`RaycastMode`](#class_n_r_kernal_1_1_n_r_input_1ad9e00319cf4326e3ad9e5a23f56fd1a9) 

Determine which raycast mode to use.

#### `{property} Transform `[`CameraCenter`](#class_n_r_kernal_1_1_n_r_input_1a706e9b4b0c14626bdc72682c9bcb6a3f) 

Get the transform of the camera which controllers are following.

#### `public const int `[`MAX_CONTROLLER_STATE_COUNT`](#class_n_r_kernal_1_1_n_r_input_1aec18a837233e50bb2a0ba96798010b21) 

Max count of controllerstates supported per frame.

# class `NRKernal::NRRenderer` 

```
class NRKernal::NRRenderer
  : public MonoBehaviour
```  

NRNativeRender oprate rendering-related things, provides the feature of ATW and low latency.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} NativeRenderring `[`m_NativeRenderring`](#class_n_r_kernal_1_1_n_r_renderer_1a285008dcbe94233cfa652dbfb975df26) | 
`public Camera `[`leftCamera`](#class_n_r_kernal_1_1_n_r_renderer_1a51bf86620865dc1f33a75129e36040c2) | 
`public Camera `[`rightCamera`](#class_n_r_kernal_1_1_n_r_renderer_1aa6dd6a89628688a4a1962722171d54a8) | 
`public inline void `[`Initialize`](#class_n_r_kernal_1_1_n_r_renderer_1a4aa10c93adef807e5b7a71be667cc40a)`(Camera leftcamera,Camera rightcamera,bool standlone)` | Initialize the render pipleline.
`public inline void `[`Pause`](#class_n_r_kernal_1_1_n_r_renderer_1a76d4f221c0d6e16d33291dad1a52d477)`()` | Pause render.
`public inline void `[`Resume`](#class_n_r_kernal_1_1_n_r_renderer_1adffc7ebb194864f768cff9d7b2e72e86)`()` | Resume render.

## Members

#### `{property} NativeRenderring `[`m_NativeRenderring`](#class_n_r_kernal_1_1_n_r_renderer_1a285008dcbe94233cfa652dbfb975df26) 

#### `public Camera `[`leftCamera`](#class_n_r_kernal_1_1_n_r_renderer_1a51bf86620865dc1f33a75129e36040c2) 

#### `public Camera `[`rightCamera`](#class_n_r_kernal_1_1_n_r_renderer_1aa6dd6a89628688a4a1962722171d54a8) 

#### `public inline void `[`Initialize`](#class_n_r_kernal_1_1_n_r_renderer_1a4aa10c93adef807e5b7a71be667cc40a)`(Camera leftcamera,Camera rightcamera,bool standlone)` 

Initialize the render pipleline.

#### Parameters
* `leftcamera` Left Eye . 

* `leftcamera` Right Eye . 

* `standlone` Whether use render without SLAM .

#### `public inline void `[`Pause`](#class_n_r_kernal_1_1_n_r_renderer_1a76d4f221c0d6e16d33291dad1a52d477)`()` 

Pause render.

#### `public inline void `[`Resume`](#class_n_r_kernal_1_1_n_r_renderer_1adffc7ebb194864f768cff9d7b2e72e86)`()` 

Resume render.

# class `NRKernal::NRRgbCamera` 

Manage the life cycle of the entire rgbcamera.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} NativeCamera `[`m_NativeCamera`](#class_n_r_kernal_1_1_n_r_rgb_camera_1a95bb7ffb806f84b9bcff8fcb8a16dcb1) | 
`public delegate void `[`CaptureEvent`](#class_n_r_kernal_1_1_n_r_rgb_camera_1a4e27acd3421f8299e9211da480ca6450)`()` | 
`public delegate void `[`CaptureErrorEvent`](#class_n_r_kernal_1_1_n_r_rgb_camera_1a66ce949bcb8410f8b152037e1f210dd1)`(string msg)` | 

## Members

#### `{property} NativeCamera `[`m_NativeCamera`](#class_n_r_kernal_1_1_n_r_rgb_camera_1a95bb7ffb806f84b9bcff8fcb8a16dcb1) 

#### `public delegate void `[`CaptureEvent`](#class_n_r_kernal_1_1_n_r_rgb_camera_1a4e27acd3421f8299e9211da480ca6450)`()` 

#### `public delegate void `[`CaptureErrorEvent`](#class_n_r_kernal_1_1_n_r_rgb_camera_1a66ce949bcb8410f8b152037e1f210dd1)`(string msg)` 

# class `NRKernal::NRSessionBehaviour` 

```
class NRKernal::NRSessionBehaviour
  : public MonoBehaviour
```  

Oprate AR system state and handles the session lifecycle for application layer.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public `[`NRSessionConfig`](#class_n_r_kernal_1_1_n_r_session_config)` `[`SessionConfig`](#class_n_r_kernal_1_1_n_r_session_behaviour_1a78ce48815ad669a044d2e3bbac83079a) | The SessionConfig of nrsession.

## Members

#### `public `[`NRSessionConfig`](#class_n_r_kernal_1_1_n_r_session_config)` `[`SessionConfig`](#class_n_r_kernal_1_1_n_r_session_behaviour_1a78ce48815ad669a044d2e3bbac83079a) 

The SessionConfig of nrsession.

# class `NRKernal::NRSessionConfig` 

```
class NRKernal::NRSessionConfig
  : public ScriptableObject
```  

A configuration used to track the world.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public bool `[`EnableATW`](#class_n_r_kernal_1_1_n_r_session_config_1afc1556148110cfe5e6b1acfb37c23c47) | 
`public TrackablePlaneFindingMode `[`PlaneFindingMode`](#class_n_r_kernal_1_1_n_r_session_config_1ac22f6fac4a30bef332b5a1027634a606) | 
`public TrackableImageFindingMode `[`ImageTrackingMode`](#class_n_r_kernal_1_1_n_r_session_config_1ab19ba963a99ba9ede5ca7d255cea155f) | 
`public `[`NRTrackingImageDatabase`](#class_n_r_kernal_1_1_n_r_tracking_image_database)` `[`TrackingImageDatabase`](#class_n_r_kernal_1_1_n_r_session_config_1a2f60f1aecfeeb1b4504c426b98564c19) | 
`public inline override bool `[`Equals`](#class_n_r_kernal_1_1_n_r_session_config_1a0c240bff465c15ebcb1e30ff003287f0)`(object other)` | ValueType check if two [NRSessionConfig](#class_n_r_kernal_1_1_n_r_session_config) objects are equal.
`public inline override int `[`GetHashCode`](#class_n_r_kernal_1_1_n_r_session_config_1aae7ae7f79f5fb7d6da1aa782ba448cf5)`()` | Return a hash code for this object.
`public inline void `[`CopyFrom`](#class_n_r_kernal_1_1_n_r_session_config_1a5773d2d5147d81ec5c631605c8942492)`(`[`NRSessionConfig`](#class_n_r_kernal_1_1_n_r_session_config)` other)` | ValueType copy from another SessionConfig object into this one.

## Members

#### `public bool `[`EnableATW`](#class_n_r_kernal_1_1_n_r_session_config_1afc1556148110cfe5e6b1acfb37c23c47) 

#### `public TrackablePlaneFindingMode `[`PlaneFindingMode`](#class_n_r_kernal_1_1_n_r_session_config_1ac22f6fac4a30bef332b5a1027634a606) 

#### `public TrackableImageFindingMode `[`ImageTrackingMode`](#class_n_r_kernal_1_1_n_r_session_config_1ab19ba963a99ba9ede5ca7d255cea155f) 

#### `public `[`NRTrackingImageDatabase`](#class_n_r_kernal_1_1_n_r_tracking_image_database)` `[`TrackingImageDatabase`](#class_n_r_kernal_1_1_n_r_session_config_1a2f60f1aecfeeb1b4504c426b98564c19) 

#### `public inline override bool `[`Equals`](#class_n_r_kernal_1_1_n_r_session_config_1a0c240bff465c15ebcb1e30ff003287f0)`(object other)` 

ValueType check if two [NRSessionConfig](#class_n_r_kernal_1_1_n_r_session_config) objects are equal.

#### Returns
True if the two [NRSessionConfig](#class_n_r_kernal_1_1_n_r_session_config) objects are value-type equal, otherwise false.

#### `public inline override int `[`GetHashCode`](#class_n_r_kernal_1_1_n_r_session_config_1aae7ae7f79f5fb7d6da1aa782ba448cf5)`()` 

Return a hash code for this object.

#### `public inline void `[`CopyFrom`](#class_n_r_kernal_1_1_n_r_session_config_1a5773d2d5147d81ec5c631605c8942492)`(`[`NRSessionConfig`](#class_n_r_kernal_1_1_n_r_session_config)` other)` 

ValueType copy from another SessionConfig object into this one.

# class `NRKernal::NRSessionManager` 

Manages AR system state and handles the session lifecycle.

Through this class, application can create a session, configure it, start/pause or stop it.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} `[`NRSessionManager`](#class_n_r_kernal_1_1_n_r_session_manager)` `[`Instance`](#class_n_r_kernal_1_1_n_r_session_manager_1a2645c4d42cb888ad672ac1d280c3e800) | 
`{property} TrackingState `[`SessionStatus`](#class_n_r_kernal_1_1_n_r_session_manager_1aa6ab661be81a04cf5b55b38e04a6b533) | 
`{property} LostTrackingReason `[`LostTrackingReason`](#class_n_r_kernal_1_1_n_r_session_manager_1a8c3de16b302941ca12babe618b853277) | 
`{property} `[`NRSessionBehaviour`](#class_n_r_kernal_1_1_n_r_session_behaviour)` `[`SessionBehaviour`](#class_n_r_kernal_1_1_n_r_session_manager_1a0da32f446f887cc9b554c63d652165c0) | 
`{property} `[`NRHMDPoseTracker`](#class_n_r_kernal_1_1_n_r_h_m_d_pose_tracker)` `[`NRHMDPoseTracker`](#class_n_r_kernal_1_1_n_r_session_manager_1ad92395c59922dc3e47eb285b6b635cc8) | 
`{property} NativeInterface `[`NativeAPI`](#class_n_r_kernal_1_1_n_r_session_manager_1a91513291451e2416ef1215bce7a3589f) | 
`{property} `[`NRRenderer`](#class_n_r_kernal_1_1_n_r_renderer)` `[`m_NRRenderringController`](#class_n_r_kernal_1_1_n_r_session_manager_1a45b2c9ba4e95e813a90b64ee7c787701) | 
`{property} bool `[`IsInitialized`](#class_n_r_kernal_1_1_n_r_session_manager_1a8f5fe4513c03b847f9426ae23eb2150d) | 
`public inline void `[`CreateSession`](#class_n_r_kernal_1_1_n_r_session_manager_1aa9013e9143ec903f7792d82aac0ba81a)`(`[`NRSessionBehaviour`](#class_n_r_kernal_1_1_n_r_session_behaviour)` session)` | 
`public inline void `[`SetConfiguration`](#class_n_r_kernal_1_1_n_r_session_manager_1a53095215c3d436a53baba94697373281)`(`[`NRSessionConfig`](#class_n_r_kernal_1_1_n_r_session_config)` config)` | 
`public inline void `[`Recenter`](#class_n_r_kernal_1_1_n_r_session_manager_1a32a20de55e7397476f08c1ac4d3fbdf7)`()` | 
`public inline void `[`StartSession`](#class_n_r_kernal_1_1_n_r_session_manager_1a9a70a960255349a7767bae2e415704a8)`()` | 
`public inline void `[`DisableSession`](#class_n_r_kernal_1_1_n_r_session_manager_1afe05e24b530268cf6e339a1b552953e7)`()` | 
`public inline void `[`ResumeSession`](#class_n_r_kernal_1_1_n_r_session_manager_1a1d3b9c5b9420c32ffd74b3e3a2d2084d)`()` | 
`public inline void `[`DestroySession`](#class_n_r_kernal_1_1_n_r_session_manager_1a0d816a80f745bf1156039bbb3ca19ba8)`()` | 

## Members

#### `{property} `[`NRSessionManager`](#class_n_r_kernal_1_1_n_r_session_manager)` `[`Instance`](#class_n_r_kernal_1_1_n_r_session_manager_1a2645c4d42cb888ad672ac1d280c3e800) 

#### `{property} TrackingState `[`SessionStatus`](#class_n_r_kernal_1_1_n_r_session_manager_1aa6ab661be81a04cf5b55b38e04a6b533) 

#### `{property} LostTrackingReason `[`LostTrackingReason`](#class_n_r_kernal_1_1_n_r_session_manager_1a8c3de16b302941ca12babe618b853277) 

#### `{property} `[`NRSessionBehaviour`](#class_n_r_kernal_1_1_n_r_session_behaviour)` `[`SessionBehaviour`](#class_n_r_kernal_1_1_n_r_session_manager_1a0da32f446f887cc9b554c63d652165c0) 

#### `{property} `[`NRHMDPoseTracker`](#class_n_r_kernal_1_1_n_r_h_m_d_pose_tracker)` `[`NRHMDPoseTracker`](#class_n_r_kernal_1_1_n_r_session_manager_1ad92395c59922dc3e47eb285b6b635cc8) 

#### `{property} NativeInterface `[`NativeAPI`](#class_n_r_kernal_1_1_n_r_session_manager_1a91513291451e2416ef1215bce7a3589f) 

#### `{property} `[`NRRenderer`](#class_n_r_kernal_1_1_n_r_renderer)` `[`m_NRRenderringController`](#class_n_r_kernal_1_1_n_r_session_manager_1a45b2c9ba4e95e813a90b64ee7c787701) 

#### `{property} bool `[`IsInitialized`](#class_n_r_kernal_1_1_n_r_session_manager_1a8f5fe4513c03b847f9426ae23eb2150d) 

#### `public inline void `[`CreateSession`](#class_n_r_kernal_1_1_n_r_session_manager_1aa9013e9143ec903f7792d82aac0ba81a)`(`[`NRSessionBehaviour`](#class_n_r_kernal_1_1_n_r_session_behaviour)` session)` 

#### `public inline void `[`SetConfiguration`](#class_n_r_kernal_1_1_n_r_session_manager_1a53095215c3d436a53baba94697373281)`(`[`NRSessionConfig`](#class_n_r_kernal_1_1_n_r_session_config)` config)` 

#### `public inline void `[`Recenter`](#class_n_r_kernal_1_1_n_r_session_manager_1a32a20de55e7397476f08c1ac4d3fbdf7)`()` 

#### `public inline void `[`StartSession`](#class_n_r_kernal_1_1_n_r_session_manager_1a9a70a960255349a7767bae2e415704a8)`()` 

#### `public inline void `[`DisableSession`](#class_n_r_kernal_1_1_n_r_session_manager_1afe05e24b530268cf6e339a1b552953e7)`()` 

#### `public inline void `[`ResumeSession`](#class_n_r_kernal_1_1_n_r_session_manager_1a1d3b9c5b9420c32ffd74b3e3a2d2084d)`()` 

#### `public inline void `[`DestroySession`](#class_n_r_kernal_1_1_n_r_session_manager_1a0d816a80f745bf1156039bbb3ca19ba8)`()` 

# class `NRKernal::NRTrackable` 

A Trackable in the real world detected by NRInternel.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline int `[`GetDataBaseIndex`](#class_n_r_kernal_1_1_n_r_trackable_1aa699caf399fd569054b3a23e917a09fa)`()` | Get the id of trackable.
`public inline TrackingState `[`GetTrackingState`](#class_n_r_kernal_1_1_n_r_trackable_1a1e16a6aa5ab7382250d3fa783cf31219)`()` | Get the tracking state of current trackable.
`public inline TrackableType `[`GetTrackableType`](#class_n_r_kernal_1_1_n_r_trackable_1a76f12b938bd9376bad3d130f7aeff1f9)`()` | Get the tracking type of current trackable.
`public inline virtual Pose `[`GetCenterPose`](#class_n_r_kernal_1_1_n_r_trackable_1af5777d0c2c1e6923a4787077367c928c)`()` | Get the center pose of current trackable.

## Members

#### `public inline int `[`GetDataBaseIndex`](#class_n_r_kernal_1_1_n_r_trackable_1aa699caf399fd569054b3a23e917a09fa)`()` 

Get the id of trackable.

#### `public inline TrackingState `[`GetTrackingState`](#class_n_r_kernal_1_1_n_r_trackable_1a1e16a6aa5ab7382250d3fa783cf31219)`()` 

Get the tracking state of current trackable.

#### `public inline TrackableType `[`GetTrackableType`](#class_n_r_kernal_1_1_n_r_trackable_1a76f12b938bd9376bad3d130f7aeff1f9)`()` 

Get the tracking type of current trackable.

#### `public inline virtual Pose `[`GetCenterPose`](#class_n_r_kernal_1_1_n_r_trackable_1af5777d0c2c1e6923a4787077367c928c)`()` 

Get the center pose of current trackable.

# class `NRKernal::NRTrackableBehaviour` 

```
class NRKernal::NRTrackableBehaviour
  : public MonoBehaviour
```  

Base classes for all trackable monobehaviour objects.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public `[`NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable)` `[`Trackable`](#class_n_r_kernal_1_1_n_r_trackable_behaviour_1afcd08b04614cac5a2c55152b72c28fe1) | 
`public inline void `[`Initialize`](#class_n_r_kernal_1_1_n_r_trackable_behaviour_1ada9501f36caf603153aa27fc5d42e945)`(`[`NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable)` trackable)` | 

## Members

#### `public `[`NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable)` `[`Trackable`](#class_n_r_kernal_1_1_n_r_trackable_behaviour_1afcd08b04614cac5a2c55152b72c28fe1) 

#### `public inline void `[`Initialize`](#class_n_r_kernal_1_1_n_r_trackable_behaviour_1ada9501f36caf603153aa27fc5d42e945)`(`[`NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable)` trackable)` 

# class `NRKernal::NRTrackableImage` 

```
class NRKernal::NRTrackableImage
  : public NRKernal.NRTrackable
```  

A trackable image in the real world detected by NRInternel.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} float `[`ExtentX`](#class_n_r_kernal_1_1_n_r_trackable_image_1ae91667c1cf8bd7856d867c8468fd55e2) | Gets the width of marker.
`{property} float `[`ExtentZ`](#class_n_r_kernal_1_1_n_r_trackable_image_1ad511fb8bd481ad3c453eb39040b15e77) | Gets the height of marker.
`{property} Vector2 `[`Size`](#class_n_r_kernal_1_1_n_r_trackable_image_1abcfadf3873f6ba3d36907ad68c517264) | Get the size of trackable image .
`public inline virtual override Pose `[`GetCenterPose`](#class_n_r_kernal_1_1_n_r_trackable_image_1a29a24bd5d33f7dd0e3304b93fb8b6888)`()` | Gets the position and orientation of the marker's center in Unity world space.

## Members

#### `{property} float `[`ExtentX`](#class_n_r_kernal_1_1_n_r_trackable_image_1ae91667c1cf8bd7856d867c8468fd55e2) 

Gets the width of marker.

#### `{property} float `[`ExtentZ`](#class_n_r_kernal_1_1_n_r_trackable_image_1ad511fb8bd481ad3c453eb39040b15e77) 

Gets the height of marker.

#### `{property} Vector2 `[`Size`](#class_n_r_kernal_1_1_n_r_trackable_image_1abcfadf3873f6ba3d36907ad68c517264) 

Get the size of trackable image .

#### Returns
size of trackable imag(width、height).

#### `public inline virtual override Pose `[`GetCenterPose`](#class_n_r_kernal_1_1_n_r_trackable_image_1a29a24bd5d33f7dd0e3304b93fb8b6888)`()` 

Gets the position and orientation of the marker's center in Unity world space.

# class `NRKernal::NRTrackableManager` 

Manages AR system state and handles the session lifecycle.

Through this class, application can create a session, configure it, start/pause or stop it.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`NRTrackableManager`](#class_n_r_kernal_1_1_n_r_trackable_manager_1a1a5d0218999a8cd50a3878f91c916d5e)`(NativeInterface nativeInterface)` | 
`public inline `[`NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable)` `[`Create`](#class_n_r_kernal_1_1_n_r_trackable_manager_1a038f8e05e25a5eb09d228235ce0bac0a)`(UInt64 trackable_handle,NativeInterface nativeInterface)` | 
`public inline void `[`GetTrackables< T >`](#class_n_r_kernal_1_1_n_r_trackable_manager_1a601b2030a82d08326b0b202ff7c00914)`(List< T > trackables,`[`NRTrackableQueryFilter`](#namespace_n_r_kernal_1a3d4c8f6767afd8d777007e814638b0e3)` filter)` | 

## Members

#### `public inline  `[`NRTrackableManager`](#class_n_r_kernal_1_1_n_r_trackable_manager_1a1a5d0218999a8cd50a3878f91c916d5e)`(NativeInterface nativeInterface)` 

#### `public inline `[`NRTrackable`](#class_n_r_kernal_1_1_n_r_trackable)` `[`Create`](#class_n_r_kernal_1_1_n_r_trackable_manager_1a038f8e05e25a5eb09d228235ce0bac0a)`(UInt64 trackable_handle,NativeInterface nativeInterface)` 

#### `public inline void `[`GetTrackables< T >`](#class_n_r_kernal_1_1_n_r_trackable_manager_1a601b2030a82d08326b0b202ff7c00914)`(List< T > trackables,`[`NRTrackableQueryFilter`](#namespace_n_r_kernal_1a3d4c8f6767afd8d777007e814638b0e3)` filter)` 

# class `NRKernal::NRTrackablePlane` 

```
class NRKernal::NRTrackablePlane
  : public NRKernal.NRTrackable
```  

A plane in the real world detected by NRInternel.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} float `[`ExtentX`](#class_n_r_kernal_1_1_n_r_trackable_plane_1a1c9b26fc6d2200f6e1592ddd246a8558) | Gets the extent of plane in the X dimension, centered on the plane position.
`{property} float `[`ExtentZ`](#class_n_r_kernal_1_1_n_r_trackable_plane_1a8ebe9e63771e420dcd0e4e8df937d674) | Gets the extent of plane in the Z dimension, centered on the plane position.
`public inline TrackablePlaneType `[`GetPlaneType`](#class_n_r_kernal_1_1_n_r_trackable_plane_1a3f1d7f8aa860d8176b895dcb0187f994)`()` | Get the plane type.
`public inline virtual override Pose `[`GetCenterPose`](#class_n_r_kernal_1_1_n_r_trackable_plane_1aa9ca8ab8c277414ca518f44e1a6e6e21)`()` | Gets the position and orientation of the plane's center in Unity world space.
`public inline void `[`GetBoundaryPolygon`](#class_n_r_kernal_1_1_n_r_trackable_plane_1a918cd3dae7d81ab4a1af5683dde25d2a)`(List< Vector3 > polygonList)` | Gets a list of points (in clockwise order) in plane coordinate representing a boundary polygon for the plane.

## Members

#### `{property} float `[`ExtentX`](#class_n_r_kernal_1_1_n_r_trackable_plane_1a1c9b26fc6d2200f6e1592ddd246a8558) 

Gets the extent of plane in the X dimension, centered on the plane position.

#### `{property} float `[`ExtentZ`](#class_n_r_kernal_1_1_n_r_trackable_plane_1a8ebe9e63771e420dcd0e4e8df937d674) 

Gets the extent of plane in the Z dimension, centered on the plane position.

#### `public inline TrackablePlaneType `[`GetPlaneType`](#class_n_r_kernal_1_1_n_r_trackable_plane_1a3f1d7f8aa860d8176b895dcb0187f994)`()` 

Get the plane type.

#### Returns
Plane type.

#### `public inline virtual override Pose `[`GetCenterPose`](#class_n_r_kernal_1_1_n_r_trackable_plane_1aa9ca8ab8c277414ca518f44e1a6e6e21)`()` 

Gets the position and orientation of the plane's center in Unity world space.

#### `public inline void `[`GetBoundaryPolygon`](#class_n_r_kernal_1_1_n_r_trackable_plane_1a918cd3dae7d81ab4a1af5683dde25d2a)`(List< Vector3 > polygonList)` 

Gets a list of points (in clockwise order) in plane coordinate representing a boundary polygon for the plane.

#### Parameters
* `polygonList` A list used to be filled with polygon points.

# class `NRKernal::NRTrackingImageDatabase` 

```
class NRKernal::NRTrackingImageDatabase
  : public ScriptableObject
```  

A database storing a list of images to be detected and tracked by NRSDK.

An image database supports up to 1000 images. Only one image database can be in use at any given time.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`{property} byte [] `[`RawData`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a0de247402810ed1540c0c537cb6ba2a2) | 
`{property} string `[`TrackingImageDataPath`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a5bc82f2b9532f50a1b33bf0aa1ce656a) | 
`{property} string `[`TrackingImageDataOutPutPath`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1aec94327be14355aa320476fd4655ca4a) | 
`{property} int `[`Count`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1aa817630d4689f7dbf3ea4391845e687e) | Gets the number of images in the database.
`{property} internal bool `[`m_IsDirty`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a6f0d89b00aa76007ebf34615edb60593) | Gets a value indicating whether the TrackingImageDatabase is dirty and has to be reset in NRSDK.
`{property} `[`NRTrackingImageDatabaseEntry`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry)` `[`this[int index]`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1aa143ddba32050b9ff427e1ccec081d06) | Gets or sets the image at the specified `index`.
`public string `[`GUID`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a2a8a9da6b9a66de2d8b49fac8f45b77f) | 
`public inline  `[`NRTrackingImageDatabase`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a88b34b4005d18d162fa39abca3d418ea)`()` | Constructs a new `TrackingImageDatabase`.

## Members

#### `{property} byte [] `[`RawData`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a0de247402810ed1540c0c537cb6ba2a2) 

#### `{property} string `[`TrackingImageDataPath`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a5bc82f2b9532f50a1b33bf0aa1ce656a) 

#### `{property} string `[`TrackingImageDataOutPutPath`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1aec94327be14355aa320476fd4655ca4a) 

#### `{property} int `[`Count`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1aa817630d4689f7dbf3ea4391845e687e) 

Gets the number of images in the database.

#### `{property} internal bool `[`m_IsDirty`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a6f0d89b00aa76007ebf34615edb60593) 

Gets a value indicating whether the TrackingImageDatabase is dirty and has to be reset in NRSDK.

#### `{property} `[`NRTrackingImageDatabaseEntry`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry)` `[`this[int index]`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1aa143ddba32050b9ff427e1ccec081d06) 

Gets or sets the image at the specified `index`.

You can only modify the database in the Unity editor. 

#### Parameters
* `index` The zero-based index of the image entry to get or set.

#### Returns
The image entry at `index`.

#### `public string `[`GUID`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a2a8a9da6b9a66de2d8b49fac8f45b77f) 

#### `public inline  `[`NRTrackingImageDatabase`](#class_n_r_kernal_1_1_n_r_tracking_image_database_1a88b34b4005d18d162fa39abca3d418ea)`()` 

Constructs a new `TrackingImageDatabase`.

# class `NRKernal::NRVersionInfo` 

Holds information about Nreal SDK version info.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `NRKernal::NRTrackingImageDatabaseEntry` 

Hold the total infomation of a image data base item.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public string `[`Name`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1aaf5187660a9db348ff47a3c7ae8d8083) | The name assigned to the tracked image.
`public float `[`Width`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1a520597fcafb7df7db0c91076b60cdfce) | The width of the image in meters.
`public string `[`Quality`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1a37295dcab61655208701e4d9f06c20f2) | The quality of the image.
`public string `[`TextureGUID`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1ae9de012d71159659269bad9f54cbf456) | The Unity GUID for this entry.
`public inline  `[`NRTrackingImageDatabaseEntry`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1a5bb62529eb265516ff27a964363a01a4)`(string name,float width)` | Contructs a new Augmented Image database entry.

## Members

#### `public string `[`Name`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1aaf5187660a9db348ff47a3c7ae8d8083) 

The name assigned to the tracked image.

#### `public float `[`Width`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1a520597fcafb7df7db0c91076b60cdfce) 

The width of the image in meters.

#### `public string `[`Quality`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1a37295dcab61655208701e4d9f06c20f2) 

The quality of the image.

#### `public string `[`TextureGUID`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1ae9de012d71159659269bad9f54cbf456) 

The Unity GUID for this entry.

#### `public inline  `[`NRTrackingImageDatabaseEntry`](#struct_n_r_kernal_1_1_n_r_tracking_image_database_entry_1a5bb62529eb265516ff27a964363a01a4)`(string name,float width)` 

Contructs a new Augmented Image database entry.

#### Parameters
* `name` The image name.

* `width` The image width in meters or 0 if the width is unknown.

Generated by [Moxygen](https://sourcey.com/moxygen)
