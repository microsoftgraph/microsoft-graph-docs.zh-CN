---
title: '已弃 (的通知资源) '
description: '表示由应用程序服务器发布的面向指定用户的通知。 通知存储在 Microsoft Graph并分发到用户拥有的不同设备终结点。 '
ms.localizationpriority: medium
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 53df1b536c20f48f9620e4e18b4f9277713d70c0
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722445"
---
# <a name="notification-resource-type-deprecated"></a>已弃 (的通知资源) 

命名空间：microsoft.graph

> [!IMPORTANT]
> Microsoft Graph 通知 API 已弃用，将在 2022 年 1 月底停止返回数据。 有关其他通知体验，请参阅 [Microsoft Azure 通知中心](/azure/notification-hubs)，并[查看此博客文章](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/)了解详细信息。

表示由应用程序服务器发布的面向指定用户的通知。 通知存储在 Microsoft Graph并分发到用户拥有的不同设备终结点。 

通知可以是可视通知有效负载，操作系统、 (Windows、Android 和 iOS 平台可以解释) 。 它还可以是传递到应用客户端 (处理的数据有效负载) 包括 Web) 的应用客户端 (Web) ，然后确定每台设备上相应的用户体验。  这通常是本地生成的可视通知 UI，对应于原始数据负载中的内容。 

当用户对可视通知操作时，应用客户端随后可以使用客户端通知 SDK 更新 Microsoft Graph 中相应通知源的状态，例如，通过将通知标记为已消除。 然后，更新将分发到所有其他应用客户端终结点，客户端会相应地处理更改，例如通过消除通知来阻止用户看到冗余信息。 应用客户端可以在过期前稍后访问同一通知资源 (即使它通过通知 [SDK](https://aka.ms/GNSDK) 标记为已) 已作为通知历史记录。 

> [!NOTE]
> 通知状态更新（如已读或已消除）不会扇出到 Web 终结点。 这是因为跨各种浏览器的 Web 推送需要向用户显示可视 Toast 通知。 由于状态更改没有相应的视觉内容，因此只会针对面向 Windows、iOS 或 Android 平台的通知扇出它们。

## <a name="methods"></a>方法

| 方法                                                   | 返回类型                                 | 说明                     |
| :------------------------------------------------------- | :------------------------------------------ | :------------------------------ |
| [创建通知](../api/user-post-notifications.md) | [notification](projectrome-notification.md) | 创建并发送通知。 |

## <a name="properties"></a>属性

| 属性           | 类型                                              | 说明                                                                                                                                                                                                                                                                                                                                               |
| :----------------- | :------------------------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| targetHostName     | String                                            | 表示呼叫服务要向其中发布通知的应用（给定用户）的主机名。 如果面向 web 终结点 (请参阅 **targetPolicy.platformTypes**) ，请确保 **targetHostName** 与在应用程序 JSON 属性内的客户端上创建订阅时所使用的名称相同。                   |
| appNotificationId  | String                                            | 应用服务器设置的唯一 ID，用于标识和定位单个通知的通知。                                                                                                                                                                                                                                     |
| groupName          | String                                            | 此通知所属的组的名称。 它由开发人员设置，用于将通知分组在一起。                                                                                                                                                                                                                   |
| targetPolicy       | [targetPolicyEndpoints](targetpolicyendpoints.md) | 目标策略对象处理针对给定用户应面向 (Windows、iOS、Android 和 WebPush) 类型的通知传递策略。                                                                                                                                                                                              |
| payload            | [payloadTypes](payloadtypes.md)                   | 这是原始或可视用户通知的数据内容，将传递给接收此通知的应用客户端并供其使用。                                                                                                                                                                                                       |
| displayTimeToLive  | Int32                                             | 设置此 (内容) 在每个平台的通知查看器中停留的秒数。 例如，当通知传递到 Windows 设备时，此属性的值将传递到 ToastNotification.ExpirationTime，该属性确定 Toast 通知将在用户的 Windows 操作中心中停留的时间。  |
| expirationDateTime | DateTimeOffset                                    | 使用 ISO 8601 格式设置用户通知的 UTC 过期日期和时间 (例如，2019 `'2019-01-01T00:00:00Z'` 年 1 月 1 日午夜 UTC 如下所示：) 。 When time is up， the notification is removed from the Microsoft Graph notification feed store and is no longer part of notification history. 最大值为 30 天。 |
| priority           | string                                            | 指示原始用户通知的优先级。 默认情况下，以高优先级发送视觉通知。 有效值为 `None`、`High` 和 `Low`。                                                                                                                                                                                                |
| fallbackPolicy     | [fallbackpolicy](fallbackpolicy.md)               | 可选回退策略对象仅处理 i (OS 终结点的通知回退策略，旨在用于由于平台特定限制（例如节电模式) ）而可能无法传递到设备的高优先级原始通知。                                                                                        |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "keyProperty": "id"
}-->

```json
{
  "targetHostName": "String",
  "appNotificationid": "String (identifier)",
  "groupName": "String", 
  "targetPolicy": {"@odata.type": "microsoft.graph.targetPolicyEndpoints"},
  "payload": {"@odata.type": "microsoft.graph.payloadTypes"},
  "displayTimeToLive": 1024,
  "expirationDateTime": "String (timestamp)",
  "priority": "string",
  "fallbackPolicy": {"@odata.type": "microsoft.graph.fallbackpolicy"} 
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
