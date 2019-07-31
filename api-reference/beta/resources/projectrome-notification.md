---
title: 通知资源类型
description: '表示由面向指定用户的应用程序服务器发布的通知。 通知存储在 Microsoft Graph 中, 并分发给用户拥有的不同设备终结点。 '
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ''
ms.openlocfilehash: f9d9a4ff77190e18b8c090cf9c976decb4edfc3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965577"
---
# <a name="notification-resource-type"></a>通知资源类型
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示由面向指定用户的应用程序服务器发布的通知。 通知存储在 Microsoft Graph 中, 并分发给用户拥有的不同设备终结点。 

通知可以是操作系统可解释的可视化通知有效负载, 包括 Windows、Android 和 iOS 平台。 它还可以是应用程序客户端传递和处理的数据有效负载, 然后在每个设备上确定相应的用户体验–通常是与生成的原始数据有效负载中的内容相对应的可视化通知 UIsmu. 

当用户在视觉通知中进行操作时, 应用程序客户端可以使用客户端 Project 罗马 SDK 更新 Microsoft Graph 中相应通知源的状态, 例如, 将通知标记为已关闭。 然后, 该更新将分发到所有其他应用程序客户端终结点, 客户端将相应地处理更改, 例如, 通过关闭通知阻止用户查看冗余信息。 应用程序客户端可以在过期之前 (甚至在将其标记为解除标记时) 访问相同的通知资源, 这是通过[Project 罗马 SDK](https://github.com/Microsoft/project-rome)的通知历史记录。 

## <a name="methods"></a>方法
|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建通知](../api/notifications-post.md) | [通告](projectrome-notification.md) |创建并发送通知。 |

## <a name="properties"></a>属性
|名称 | 类型 | 说明|
|:----|:-----|:-----------|
| targetHostName | String | 表示呼叫服务要为其发布通知的应用程序的主机名 (针对给定用户)。 |
| appNotificationId | String | 通知的应用程序服务器设置的唯一 id, 用于标识和定位单个通知。 |
| expirationDateTime | DateTimeOffset | 在用户通知上设置 UTC 过期时间-当时间启动时, 将从 Microsoft Graph 通知源存储中完全删除通知, 并且不再是通知历史记录的一部分。 最大值为30天。 |
| payload | Edm、JSON 对象 | 这是原始或直观的用户通知的数据内容, 这些通知将传递给应用客户端接收此通知并由其使用。 |
| rawContent | String | 原始用户通知的通知内容, 该通知内容将传递给应用程序客户端接收此通知并由其使用。 RawContent 和 VisualContent 中至少有一个有效的和需要对 POST 通知请求有效。 |
| 有效负载。 visual | Edm、JSON 对象 | 直观用户通知的可视内容, 它将由每个移动平台上的通知平台使用, 并为用户呈现。 至少有一个内容和 VisualContent 需要对 POST 通知请求有效。 |
| 有效负载. 标题 | String | 可视用户通知的标题。 必须具有 "标题" 或 "正文"。 |
| 有效负载 | String | 可视化用户通知的正文。 必须具有 "标题" 或 "正文"。 |
| displayTimeToLive | Int | 设置此通知内容将在每个平台的通知查看器中保留多长时间 (以秒为单位)。 例如, 将通知传递给 Windows 设备时, 此属性的值将传递给 ToastNotification, 以确定 toast 通知将在用户的 Windows 操作中心保留多长时间。 |
| priority | EnumType | 指示原始用户通知的优先级。 默认情况下, 视觉通知以高优先级发送。 有效值为 "高" 和 "低"。 |
| 名 | String | 此通知所属的组的名称。 它由开发人员设置, 用于将通知分组在一起。 |
| targetPolicy | Edm、JSON 对象 | 目标策略对象在两个不同的级别 (应针对其目标的终结点类型 (Windows、iOS 和 Android) 以及应针对目标的特定终结点 (由订阅 id 标识) 中处理通知传递策略。 |
| targetPolicy.platformTypes | Edm、集合 (EnumType) | 使用将通知分发筛选到特定平台或平台。 默认情况下, 将启用所有 "推送终结点类型" (iOS、Windows 和 Android)。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
以下是在发布传递到目标操作系统的直接直观通知时, 资源的 JSON 表示形式。

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

以下是在发布传递给应用程序客户端的原始数据通知时的资源的 JSON 表示形式。
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
