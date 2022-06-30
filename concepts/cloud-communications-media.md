---
title: 使用云通信 API 选择媒体托管选项
description: 使用 Microsoft Graph 中的云通信 API 选择媒体托管选项，使机器人能够发送和接收与音频和视频相关的内容。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: d0178fe09668c2199ec2a985ff7df89d36d1d02f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440997"
---
# <a name="choose-a-media-hosting-option"></a>选择媒体托管选项

使用 Microsoft Graph 中的云通信 API 使机器人能够发送和接收与音频和视频相关的内容。 通过使用媒体，可以在机器人和用户之间创建更具交互性的体验。

本文可帮助你根据需要确定适合自己的媒体托管选项：服务托管媒体或应用程序托管媒体。

## <a name="service-hosted-media-remote-hosting"></a>服务托管媒体 (远程托管) 

如果希望机器人在客户拨号业务号码时播放自定义提示，或检测电话音调、录制短语音剪辑或执行任何各种交互式语音响应 ([IVR](/graph/api/resources/calls-api-ivr-overview)) 方案，请考虑使用 [服务托管媒体 API](/graph/api/resources/communications-api-overview)。

**如果媒体需求更简单，请先浏览此选项**。 由于重介质处理是远程卸载的，因此这是一种重量较轻的解决方案，可用于以更灵活的方式生成机器人。

有关演示如何创建使用服务托管媒体的机器人的示例，请参阅 [远程媒体调用机器人示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/RemoteMediaSamples)。

![远程托管关系图](images/communications-remote-media.PNG)

## <a name="application-hosted-media-local-hosting"></a>应用程序托管媒体 (本地托管) 

如果希望机器人通过自然语言处理服务访问用于录制、转录、翻译或情绪分析的客户音频和视频的实时流，请考虑在本地托管媒体。

> [!IMPORTANT]
> **不能** 使用媒体访问 API 记录或以其他方式保存来自应用程序访问的呼叫或会议的媒体内容，或从该媒体内容派生的数据 (“记录”或“录制”) ，而无需先调用 [updateRecordingStatus API](/graph/api/call-updaterecordingstatus) 来指示录制已经开始，并从该 API 收到成功回复。
>
> 如果应用程序开始录制任何会议/电话，则必须在调用 updateRecordingStatus API 之前结束录制，以指示录制已结束。 确保遵守有关数据保护和通信保密性的相关法律和法规。 有关详细信息，请参阅 [使用条款](/legal/microsoft-apis/terms-of-use) 并咨询您的法律顾问。

**如果希望更好地控制媒体，请选择此选项**。 你将直接访问媒体流，并能够使用基于视频的屏幕共享。 你将能够生成启用语音的更复杂的 IVR 方案。 这是一个较重的权重解决方案，让你在媒体编程方式上具有最大的灵活性。

另请参阅应用程序托管媒体机器人 [的要求和注意](/microsoftteams/platform/concepts/calls-and-meetings/requirements-considerations-application-hosted-media-bots) 事项。

有关演示如何创建使用应用程序托管媒体的机器人的示例，请参阅 [本地媒体示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/LocalMediaSamples)。

![本地托管图](images/communications-local-media.PNG)

## <a name="see-also"></a>另请参阅

- [通话权限](./permissions-reference.md#calls-permissions)
- [云通信 API 概述](cloud-communications-concept-overview.md)