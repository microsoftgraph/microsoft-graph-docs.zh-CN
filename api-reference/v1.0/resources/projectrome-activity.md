---
title: 活动资源类型
description: 表示应用中的单个活动 -例如，电视节目、文档或游戏中的当前活动。 当用户参与该活动时，该活动将捕获为指示该活动的开始时间和结束时间的历史项。 随着用户随着时间的过去重新参与该活动，将针对单个用户活动记录多个历史记录项。
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 06dfcd951826e65fc8c781b84156d89e542df370
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028791"
---
# <a name="activity-resource-type"></a>活动资源类型

命名空间：microsoft.graph

表示应用中的单个活动 -例如，电视节目、文档或游戏中的当前活动。 当用户参与该活动时，该活动将捕获为指示该活动的开始时间和[](projectrome-historyitem.md)结束时间的历史项。 随着用户随着时间的过去重新参与该活动，将针对单个用户活动记录多个历史记录项。

可以使用 Microsoft Graph中的活动，以便用户跨多台设备重新回到他们在应用中所执行的活动。 你的应用创建的活动显示在所有用户的设备上，并作为指向应用中特定内容的深层链接向用户公开。 你可以将应用中的特定内容表示为在 Windows 中展示的目标，并通过通知在 iOS 和 Android Cortana访问。

由于每个应用都不同，因此由你了解将应用程序中的操作映射到将在"日程表"和"日程表"Cortana活动的最佳方法。 例如，游戏可能会为每个市场活动创建一个活动，文档创作应用可能会为每个唯一文档创建一个活动，业务线应用可能会为每个工作流创建一个活动。

你的用户活动将在 Cortana 和 Windows Timeline 用户体验中展示，它们侧重于通过帮助用户恢复过去处理的内容来提高工作效率。

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建或替换活动](../api/projectrome-put-activity.md) | [活动](projectrome-activity.md) |创建或替换现有活动 (upsert) 。 appActivityId 必须是 URL 安全字符 (除 RFC 2396 未保留字符之外的所有字符都必须转换为其十六进制表示形式) ，但原始 appActivityId 不一定是 URL 安全字符。 |
|[删除活动](../api/projectrome-delete-activity.md) | 无内容 | 从你的应用中删除该用户的指定活动。|
|[获取活动](../api/projectrome-get-activities.md) | 活动 [集合](projectrome-activity.md) | 获取给定用户的应用活动。|
|[获取最近的活动](../api/projectrome-get-recent-activities.md) | 活动 [集合](projectrome-activity.md) | 获取给定用户的应用的最新活动，根据最近创建或更新的 [historyItems 排序和排序](projectrome-historyitem.md)。|

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|userTimezone | String | 可选。 用户用于生成活动的设备在活动创建时所在的时区;值作为 Olson IDs 提供，以支持跨平台表示。|
|createdDateTime | DateTimeOffset | 由服务器设置。 在服务器上创建对象时的日期/时间（UTC 时间）。 |
|lastModifiedDateTime | DateTimeOffset | 由服务器设置。 在服务器上修改对象的 DateTime（UTC 时间）。 |
|id | String | 用于 URL 寻址的服务器生成的 ID。|
|appActivityId | String | 必填。 应用上下文中的唯一活动 ID - 由调用方提供，此后不可变。|
|activitySourceHost | String | 必填。 表示应用的跨平台标识映射的域的 URL。 映射存储为托管在域上的 JSON 文件，或可通过 Windows 开发人员中心。 JSON 文件命名为跨平台应用标识符，并托管在 HTTPS 域的根目录（顶级域）或包含子域。 例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。 每个跨平台应用标识 (一个唯一的文件和) 子域。 例如，Word 和 Word 应用程序需要单独的文件和PowerPoint。|
|appDisplayName | String | 可选。 用于在用户的本地设备上未安装应用时生成活动以使用的应用的简短文本说明。|
|activationUrl | String | 必填。 用于以 appId 表示的最佳本机体验启动活动的 URL。 如果不存在本机应用，则可能会启动基于 Web 的应用。|
|fallbackUrl | String | 可选。 用于在基于 Web 的应用中启动活动的 URL（如果可用）。|
|contentUrl | String | 可选。 在内容可以在本机或基于 Web 的应用体验之外呈现时使用 (例如，指向 RSS 源中的项的指针) 。|
|visualElements| [visualInfo](../resources/projectrome-visualinfo.md) | 必需。 包含在 UX 中呈现活动的信息的对象。|
|contentInfo | 未键入的 JSON 对象 | 可选。 一条自定义数据 - JSON-LD 根据自定义语法对内容 schema.org[说明。](https://schema.org)|
|expirationDateTime | DateTimeOffset | 由服务器设置。 对象在服务器上过期时的日期/时间（UTC 时间）。|
|status | status | 由服务器设置。 用于标识有效对象的状态代码。 值：活动、已更新、已删除、已忽略。|

## <a name="relationships"></a>关系

|关系 | 类型 | 说明|
|:------------|:-----|:-----------|
|historyItems| [activityHistoryItem](../resources/projectrome-historyitem.md) 集合 | 可选。 NavigationProperty/包含;活动 historyItems 的导航属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "appDisplayName",
    "fallbackUrl",
    "contentUrl",
    "contentInfo",
    "visualElements",
    "historyItems"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.userActivity",
  "@odata.annotations": [
    {
      "capabilities": {
        "countable": false,
        "selectable": false,
        "skippable": false
      }
    }
  ]
}-->

```json
{
    "appActivityId": "String",
    "activitySourceHost": "String (host name/domain/URL)",
    "userTimezone": "String",
    "appDisplayName": "String",
    "activationUrl": "String (URL)",
    "contentUrl": "String (URL)",
    "fallbackUrl": "String (URL)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "expirationDateTime": "DateTimeOffset",
    "id": "String",
    "status": "active | updated | deleted | ignored",
    "contentInfo": { "@odata.type": "microsoft.graph.Json" },
    "visualElements": { "@odata.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.activityHistoryItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

