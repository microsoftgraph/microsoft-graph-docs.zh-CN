---
title: 通知资源类型
description: '代表由指定的用户的目标应用程序服务器发布的通知。 通知存储在 Microsoft Graph 中并分发到不同设备用户所拥有的终结点。 '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509257"
---
# <a name="notification-resource-type"></a>通知资源类型
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表由指定的用户的目标应用程序服务器发布的通知。 通知存储在 Microsoft Graph 中并分发到不同设备用户所拥有的终结点。 

通知可以是可由操作系统，包括 Windows、 Android 和 iOS 平台解释 visual 通知负载。 也可以是数据负载的已送达和处理应用程序的客户端，然后确定相应的用户体验上每个设备 – 通常情况下，visual 通知对应于中生成的原始数据有效负载的内容的 UI本地。 

当用户对 visual 通知时，应用程序客户端然后可以使用客户端项目 Rome SDK 更新的源中 Microsoft Graph-例如，通过将通知标记为消除相应通知状态。 更新将随后可分配给所有其他应用程序客户端终结点，并在客户端更改据此处理，例如通过消除该通知以防止用户看到冗余信息。 应用程序客户端可以在以后到期 （即使该被标记为消除） 之前, 访问相同的通知资源作为通知历史记录，通过[Project Rome SDK](https://github.com/Microsoft/project-rome)。 

## <a name="methods"></a>方法
|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建通知](../api/projectrome-notification-post.md) | 通知 |创建和发送通知。 |

## <a name="properties"></a>属性
|名称 | 类型 | 说明|
|:----|:-----|:-----------|
| targetHostName | String | 代表调用服务希望发布的给定用户的通知应用程序的主机名。 |
| appNotificationId | String | 设置用于标识和目标单个通知的通知的应用程序服务器的唯一 id。 |
| expirationDateTime | DateTimeOffset | 设置 UTC 过期时间用户通知的时间时，通知已从 Microsoft Graph 通知源存储完全并且不再通知历史记录的一部分。 最大值为 30 天。 |
| payload | Edm.ComplexType，JSON 对象 | 这是将传递到和使用应用程序客户端接收该通知的原始或 visual 用户通知的数据内容。 |
| payload.rawContent | String | 将传递到和使用应用程序客户端接收该通知的原始用户通知通知内容。 至少一个 Payload.RawContent 和 Payload.VisualContent 需要有效 POST 通知请求。 |
| payload.visual | Edm.ComplexType，JSON 对象 | Visual 可视化用户通知，其中将使用每个移动平台上的通知平台和呈现的用户的内容。 至少一个内容和 VisualContent 需要有效 POST 通知请求。 |
| payload.visual.title | String | 可视化用户通知的标题。 必须具有标题或正文。 |
| payload.visual.body | String | 可视化用户通知的正文。 必须具有标题或正文。 |
| displayTimeToLive | Int | 设置多长时间 （以秒为单位） 此通知内容将保持在每个平台通知查看器中。 例如，通知传递到 Windows 设备，此属性的值被传递到 ToastNotification.ExpirationTime，确定长吐司通知将保持在用户的 Windows 操作中心。 |
| priority | EnumType | 指示原始用户通知的优先级。 默认情况下，visual 通知发送高优先级。 有效值为上限和下限。 |
| GroupName | String | 此通知所属的组的名称。 它通过将通知组合在一起以开发人员进行设置。 |
| targetPolicy | Edm.ComplexType，JSON 对象 | 目标策略对象处理在两个不同级别的目标应该的终结点类型 （Windows、 iOS 和 Android） 和特定的终结点 （由订阅 id 标识） 的目标应该通知传递策略。 |
| targetPolicy.platformTypes | Edm.ComplexType，集合 (EnumType) | 用于筛选通知分发给特定平台或平台。 默认情况下，启用所有推送终结点类型 （iOS、 Windows 和 Android）。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的当您发布送达目标操作系统的直接可视化通知的 JSON 表示形式。

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

下面是资源的当您发布传递到应用程序客户端的原始数据通知的 JSON 表示形式。
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-notification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
