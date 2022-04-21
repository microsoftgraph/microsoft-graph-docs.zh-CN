---
title: 使用 Microsoft Graph 云通信 API 时，确定名册中的大型库视图参与者
description: 了解如何识别名册中的大型库视图参与者。
author: navali-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 0d4c0912080c7d6d24bfe8f0b450efe338c89deb
ms.sourcegitcommit: 4ff6e89e89178cbd5aef8aa019e714d95817fae4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2022
ms.locfileid: "65017014"
---
# <a name="identify-large-gallery-view-participants-in-a-roster-when-using-the-microsoft-graph-cloud-communications-api"></a>使用 Microsoft Graph 云通信 API 时，确定名册中的大型库视图参与者

云通信 API 提供了一个终结点，用于将 [大型库视图添加](/graph/api/call-addlargegalleryview) 到调用。 将大型库视图成功添加到呼叫后，可以订阅参与者的视频源。

本文介绍如何识别名册中的大型库视图参与者，以便可以检索相关数据以订阅视频源。

## <a name="roster-example-with-large-gallery-view-participant"></a>具有大型库视图参与者的花名册示例

以下示例演示应用程序在大型库视图成功添加到调用后收到的名册。

```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/5f201300-df95-4800-bd3a-75b0af63dd2b/participants",
      "resourceUrl": "/communications/calls/5f201300-df95-4800-bd3a-75b0af63dd2b/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "displayName": "(redacted)",
                "identityProvider": "AAD",
              }
            },
            "endpointType": "default",
            "endpointId": "40213cfb-0934-4dce-9b3a-57c09adf6967",
            "participantId": "23aeb644-6227-4f4a-b5c9-4d61c1f196d3",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2472",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "meetingRole": "presenter",
          "id": "23aeb644-6227-4f4a-b5c9-4d61c1f196d3"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "displayName": "(redacted)",
                "identityProvider": "AAD"
              }
            },
            "endpointType": "default",
            "endpointId": "4a767d9b-dca5-4176-8f1b-2a0f98923569",
            "participantId": "63ce9188-e754-4733-9e71-ccc829499a63",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1652",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "1653",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "1655",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "data",
              "label": "data",
              "sourceId": "1656",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "meetingRole": "presenter",
          "id": "63ce9188-e754-4733-9e71-ccc829499a63"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "identityProvider": "AAD",
                "ApplicationType": "LargeGallery-V2"
              }
            },
            "endpointType": "default",
            "endpointId": "ccf24195-bd6d-4cbe-bc46-180a7fd3e9ba",
            "participantId": "a34eae65-7aca-43ab-8332-80ab28629a54",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2886",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "2887",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "metadata": "{\"__platform\":{\"ui\":{\"hidden\":true}},\"audienceView\":{\"id\":\"3c28fd97-6d51-4f2f-8bba-82dcbf408ff6/1\",\"page\":1,\"status\":\"active\",\"type\":\"lg\",\"aspectRatio\":\"widescreen\"}}",
          "isMuted": false,
          "isInLobby": false,
          "meetingRole": "presenter",
          "id": "a34eae65-7aca-43ab-8332-80ab28629a54"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "identityProvider": "AAD",
                "ApplicationType": "LargeGallery-V2"
              }
            },
            "endpointType": "default",
            "endpointId": "22726e72-fbf4-46c7-a5d7-36c682c3ba86",
            "participantId": "8c4ca6bc-33e1-4da5-b6d6-a2fe61af605d",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2673",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "2674",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "data",
              "label": "data",
              "sourceId": "2685",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "metadata": "{\"__platform\":{\"ui\":{\"hidden\":true}}}",
          "isMuted": false,
          "isInLobby": false,
          "meetingRole": "presenter",
          "id": "8c4ca6bc-33e1-4da5-b6d6-a2fe61af605d"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "displayName": "(redacted)",
                "identityProvider": "AAD"
              }
            },
            "endpointType": "default",
            "endpointId": "c2bba3c4-ffff-ffff-eca6-782d381190f4",
            "participantId": "3855ce6a-064e-402c-a1cf-2d78b4e1efbb",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "201",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "202",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "212",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "data",
              "label": "data",
              "sourceId": "213",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "metadata": "{\"holographicCapabilities\":3}",
          "isMuted": true,
          "isInLobby": false,
          "meetingRole": "organizer",
          "id": "3855ce6a-064e-402c-a1cf-2d78b4e1efbb"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "displayName": "(redacted)",
                "identityProvider": "AAD"
              }
            },
            "endpointType": "default",
            "endpointId": "b8e00934-5ae7-4e8b-9933-1ed41d70e8c0",
            "participantId": "f65b97d2-efda-471e-a2c5-bfe40146b11f",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2267",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "2268",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "2270",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "data",
              "label": "data",
              "sourceId": "2271",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "publishedStates": [],
          "meetingRole": "presenter",
          "id": "f65b97d2-efda-471e-a2c5-bfe40146b11f"
        }
      ]
    }
  ]
}
```

## <a name="identifying-large-gallery-view-participants"></a>标识大型库视图参与者

使用名册示例中的以下数据标识大型库视图参与者：

- 参与者的 **ApplicationType** 将设置为 `LargeGallery-V2`。
- 视频媒体流 **的方向** 将设置为 `sendReceive`。
- 将包含元 **数据** ，其中将包含更多详细信息，例如分页。

### <a name="participant-data-example"></a>参与者数据示例

以下示例显示了名册中大型库视图参与者的数据。

```json
{
    "@odata.type": "#microsoft.graph.participant",
    "info": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "application": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "(redacted)",
        "identityProvider": "AAD",
        "ApplicationType": "LargeGallery-V2"
        }
    },
    "endpointType": "default",
    "endpointId": "ccf24195-bd6d-4cbe-bc46-180a7fd3e9ba",
    "participantId": "a34eae65-7aca-43ab-8332-80ab28629a54",
    },
    "mediaStreams": [
    {
        "@odata.type": "#microsoft.graph.mediaStream",
        "mediaType": "audio",
        "label": "main-audio",
        "sourceId": "2886",
        "direction": "receiveOnly",
        "serverMuted": false
    },
    {
        "@odata.type": "#microsoft.graph.mediaStream",
        "mediaType": "video",
        "label": "main-video",
        "sourceId": "2887",
        "direction": "sendReceive",
        "serverMuted": false
    }
    ],
    "metadata": "{\"__platform\":{\"ui\":{\"hidden\":true}},\"audienceView\":{\"id\":\"3c28fd97-6d51-4f2f-8bba-82dcbf408ff6/1\",\"page\":1,\"status\":\"active\",\"type\":\"lg\",\"aspectRatio\":\"widescreen\"}}",
    "isMuted": false,
    "isInLobby": false,
    "meetingRole": "presenter",
    "id": "a34eae65-7aca-43ab-8332-80ab28629a54"
}
```

### <a name="definition-for-deserializing-metadata"></a>反序列化元数据的定义

使用以下定义反序列化 **元数据** 属性并提取相关信息。

```csharp
    /// <summary>
    /// Metadata for large gallery view
    /// </summary>
    [DataContract]
    public class AudienceView
    {
        /// <summary>
        /// Unique view id
        /// </summary>
        [DataMember(Name = "id")]
        public string Id { get; set; }

        /// <summary>
        /// Page Number
        /// </summary>
        [DataMember(Name = "page")]
        public int Page { get; set; }

        /// <summary>
        /// Signal that page is Active/Inactive
        /// </summary>
        [DataMember(Name = "status")]
        public string Status { get; set; }
    }
```

