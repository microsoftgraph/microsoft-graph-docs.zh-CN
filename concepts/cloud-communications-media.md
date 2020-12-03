---
title: 媒体概述
description: 使你的 bot 能够发送和接收与音频和视频相关的内容。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 74738233915f0a0731790ee8b0646f437585cb67
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522424"
---
# <a name="media-overview"></a>媒体概述

Microsoft Graph 中的云通信 Api 为您的应用和服务如何通过各种通信相关功能（如呼叫和联机会议）与用户进行交互，从而添加了一个新的维度。 您可以启用您的 bot 以发送和接收与音频和视频相关的内容。 通过使用媒体，你可以在你的 bot 和用户之间创建更具交互性的体验。

本文将帮助您根据自己的需要，发现哪种媒体承载选项适合您。

## <a name="service-hosted-media-remote-hosting"></a>服务承载的媒体 (远程托管) 
如果您希望您的 bot 在客户拨打您的公司号码时播放自定义提示，或者要检测电话音，请记录短语音剪辑，或在 IVR 中执行任何不同的交互语音响应 ([IVR](/graph/api/resources/calls-api-ivr-overview)) 方案，请考虑使用[服务托管的媒体 api](/graph/api/resources/communications-api-overview)。

**如果你的媒体需求更简单，请先浏览此选项**。 由于远程卸载了重型媒体处理，因此这是一个较轻重量的解决方案，可让你以更灵活的方式构建你的 bot。

有关演示如何创建使用服务托管媒体的 bot 的示例，请参阅 [远程媒体呼叫机器人示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples)。

![远程承载关系图](images/communications-remote-media.PNG)

## <a name="application-hosted-media-local-hosting"></a>应用程序承载的媒体 (本地托管) 
如果您希望您的 bot 访问客户的音频和视频流，以用于通过自然语言处理服务录制、转录、翻译或看法分析，请考虑在本地托管媒体。

>**注意：** 您 **不能** 使用媒体访问 API，在您的应用程序访问的呼叫或会议中或从该媒体 )  ( 内容派生的数据中保留媒体内容，而无需先调用 [updateRecordingStatus API](/graph/api/call-updaterecordingstatus) 来指示录制已开始，并从该 api 接收成功答复。 如果您的应用程序开始录制任何会议/呼叫，则它必须在调用 updateRecordingStatus API 之前结束录制，以指示录制已结束。 请确保您符合有关通信的数据保护和机密性的法律和法规。 有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。

**如果您希望更好地控制媒体，请选择此选项**。 你将能够直接访问媒体流，并且可以使用基于视频的屏幕共享。 你将能够生成启用了语音的更复杂的 IVR 方案。 这是一个较重的解决方案，为你提供了对媒体编程方式的最大灵活性。

另请参阅应用程序托管媒体 bot 的 [要求和注意事项](/microsoftteams/platform/concepts/calls-and-meetings/requirements-considerations-application-hosted-media-bots) 。

有关演示如何创建使用应用程序承载的媒体的 bot 的示例，请参阅 [本地媒体示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/LocalMediaSamples)。

![本地承载关系图](images/communications-local-media.PNG)

## <a name="see-also"></a>另请参阅

- [通话权限](./permissions-reference.md#calls-permissions)
