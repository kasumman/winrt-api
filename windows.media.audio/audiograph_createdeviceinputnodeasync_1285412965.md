---
-api-id: M:Windows.Media.Audio.AudioGraph.CreateDeviceInputNodeAsync(Windows.Media.Capture.MediaCategory,Windows.Media.MediaProperties.AudioEncodingProperties)
-api-type: winrt method
---

<!-- Method syntax
public Windows.Foundation.IAsyncOperation<Windows.Media.Audio.CreateAudioDeviceInputNodeResult> CreateDeviceInputNodeAsync(Windows.Media.Capture.MediaCategory category, Windows.Media.MediaProperties.AudioEncodingProperties encodingProperties)
-->

# Windows.Media.Audio.AudioGraph.CreateDeviceInputNodeAsync

## -description
Creates an [AudioDeviceInputNode](audiodeviceinputnode.md) that inputs audio data into the audio graph from the default audio input device such as a microphone or audio card.

## -parameters
### -param category
A value from the [MediaCategory](../windows.media.capture/mediacategory.md) enumeration value indicating the category of the media processed by this node, allowing the system to perform content-appropriate processing and prioritization of the media.

### -param encodingProperties
An object representing the audio encoding properties for the device input node which specifies the sample rate at which the created node will operate. Only uncompressed PCM and float formats are allowed.

## -returns
An asynchronous operation that returns a [CreateAudioDeviceInputNodeResult](createaudiodeviceinputnoderesult.md) on completion. This object exposes a [Status](createaudiodeviceinputnoderesult_status.md) property, that indicates either that the operation was successful or the reason why the operation failed. The [DeviceInputNode](createaudiodeviceinputnoderesult_deviceinputnode.md) property provides a reference to the created input node on success.

## -remarks
Other overloads of this method allow you to specify the ID of a specific audio device instead of using the system's default device.

## -examples

## -see-also
[CreateDeviceInputNodeAsync(MediaCategory)](audiograph_createdeviceinputnodeasync_420106269.md), [CreateDeviceInputNodeAsync(MediaCategory, AudioEncodingProperties, DeviceInformation)](audiograph_createdeviceinputnodeasync_757181607.md)
## -capabilities
backgroundMediaRecording
