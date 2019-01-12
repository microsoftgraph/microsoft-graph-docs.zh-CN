---
title: 活动资源类型
description: 表示应用程序-例如，TV 显示、 文档或视频游戏中的当前市场活动中的单个活动。 当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。 根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: eade448e9585ac3678c81548c242bd467e71df40
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991074"
---
# <a name="activity-resource-type"></a>活动资源类型

表示应用程序-例如，TV 显示、 文档或视频游戏中的当前市场活动中的单个活动。 当用户启动与该活动时，此服务捕获作为[历史记录项](projectrome-historyitem.md)，指示该活动的开始和结束时间。 根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。

您可以使用在 Microsoft Graph 活动使用户能够获得到它们在做什么其应用程序中跨多个设备。 您的应用程序创建的活动显示所有用户在设备上，并向用户公开为深度链接到您的应用程序中的特定内容。 您可以为在 Windows 中，并在 iOS 和通过 Cortana 通知 Android 设备上访问展示的目标应用程序中表示特定内容。

由于每个应用程序不同，这取决于您了解映射中将出现在 Cortana 和日程表的用户活动应用程序的操作的最佳方式。 例如，游戏可能创建活动的每个市场活动、 文档创作应用程序可能会创建每个唯一的文档，活动和业务线应用程序可能会创建每个工作流活动。

用户活动将供展示中 Cortana 和 Windows 时间线用户体验，重点以帮助其选择回到从事过去的内容来提高用户工作效率和效率。

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建或替换活动](../api/projectrome-put-activity.md) | [活动](projectrome-activity.md) |创建或替换现有的活动 (upsert)。 AppActivityId 需要 URL 安全 （除 RFC 2396 必须将未保留的字符转换为十六进制表示形式为所有字符），但原始 appActivityId 不必是安全的 URL。 |
|[删除活动](../api/projectrome-delete-activity.md) | 无内容 | 从您的应用程序中删除指定为该用户的活动。|
|[获取活动](../api/projectrome-get-activities.md) | [活动](projectrome-activity.md)的集合 | 获取指定用户的应用程序的活动。|
|[获取最近的活动](../api/projectrome-get-recent-activities.md) | [活动](projectrome-activity.md)的集合 | 为给定的用户、 排序和基于[historyItems](projectrome-historyitem.md)最近创建或更新您的应用程序获取最新的活动。|

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|userTimezone | 字符串 | 可选。 在其中用于生成活动的用户的设备已位于在活动创建时; timezone为了支持跨平台表示形式作为 Olson Id 提供的值。|
|createdDateTime | DateTimeOffset | 由服务器设置。 采用 UTC 的服务器上创建对象时的日期和时间。 |
|lastModifiedDateTime | DateTimeOffset | 由服务器设置。 采用 UTC 的服务器上修改对象时的日期和时间。 |
|id | 字符串 | 使用的 URL 地址的服务器生成的 ID。|
|appActivityId | 字符串 | 必需。 应用程序-此后提供呼叫者和不可变的上下文中唯一的活动 ID。|
|activitySourceHost | 字符串 | 必需。 表示应用程序的跨平台标识映射的域的 URL。 映射是存储也为 JSON 文件域上托管或通过 Windows 开发人员中心可配置。 JSON 文件命名为跨平台应用程序标识符和承载在您的 HTTPS 域，在顶级域根目录或包括 sub 域。 例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。 您必须具有唯一文件和域 （或 sub 域），每个跨平台应用程序标识。 例如，Word 与 PowerPoint 的需要单独的文件和域。|
|appDisplayName | 字符串 | 可选。 用于生成使用活动情况下，用户的本地设备上未安装应用程序时应用程序的简短的文本说明。|
|activationUrl | 字符串 | 必需。 用于启动最佳本机体验由 appId 中的活动 URL。 如果没有的本机应用程序存在，则可能会启动一个基于 web 的应用程序。|
|fallbackUrl | 字符串 | 可选。 用于启动基于 web 的应用程序中的活动如果可用的 URL。|
|contentUrl | 字符串 | 可选。 使用在事件的内容可以呈现之外的本机或基于 web 的应用程序体验 （例如，RSS 源中的项目的指针）。|
|visualElements| [visualInfo](../resources/projectrome-visualinfo.md) | 必填。 包含信息呈现体验中的活动的对象|
|contentInfo | 类型化的 JSON 对象 | 可选。 一个自定义的数据的 JSON LD 根据[schema.org](https://schema.org)语法的内容的可扩展说明。|
|expirationDateTime | DateTimeOffset | 由服务器设置。 采用 UTC 对象过期的服务器上时的日期和时间。|
|status | status | 由服务器设置。 一个用于标识有效对象的状态代码。 值： 活动更新、 删除、 忽略。|

## <a name="relationships"></a>Relationships

|关系 | 类型 | 说明|
|:------------|:-----|:-----------|
|historyItems| [activityHistoryItem](../resources/projectrome-historyitem.md)集合 | 可选。 NavigationProperty/包容;导航到活动的 historyItems 属性。|

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
