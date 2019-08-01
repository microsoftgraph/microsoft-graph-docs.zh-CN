---
title: 活动资源类型
description: 代表某个应用程序内的单个活动, 例如电视节目、文档或视频游戏中的当前市场活动。 当用户参与该活动时, 会将该预订作为历史项目进行捕获, 以指示该活动的开始时间和结束时间。 随着时间的推移, 用户随着时间的推移而重新参与该活动, 会为单个用户活动记录多个历史记录项目。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 1b0e0f7cd6ed3a7629653719078b1e69eeeffc19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035026"
---
# <a name="activity-resource-type"></a>活动资源类型

代表某个应用程序内的单个活动, 例如电视节目、文档或视频游戏中的当前市场活动。 当用户参与该活动时, 会将该预订作为[历史项目](projectrome-historyitem.md)进行捕获, 以指示该活动的开始时间和结束时间。 随着时间的推移, 用户随着时间的推移而重新参与该活动, 会为单个用户活动记录多个历史记录项目。

您可以使用 Microsoft Graph 中的活动来使用户能够返回到在其应用程序中的多个设备上执行的操作。 您的应用程序创建的活动将显示在所有用户的设备上, 并向用户公开为您的应用程序中的特定内容的深层链接。 您可以将应用程序中的特定内容表示为在 Windows 中 showcased 的目标, 并通过 Cortana 通知在 iOS 和 Android 设备上访问。

由于每个应用程序都不同, 因此您可以了解将应用程序内的操作映射到将在 Cortana 和时间线中显示的用户活动的最佳方式。 例如, 游戏可能会为每个市场活动创建一个活动, 文档创作应用程序可能会为每个唯一文档创建一个活动, 并且业务线应用程序可能会为每个工作流创建一个活动。

你的用户活动将 showcased 在 Cortana 和 Windows 时间线用户体验中, 这主要是为了提高用户的工作效率和效率, 因为它可帮助他们获取过去对用户的工作内容。

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建或替换活动](../api/projectrome-put-activity.md) | [活动](projectrome-activity.md) |创建或替换现有活动 (upsert)。 AppActivityId 需要是 URL 安全的 (除 RFC 2396 非保留字符之外的所有字符都必须转换为十六进制表示形式), 但原始 appActivityId 不必是 URL 安全的。 |
|[删除活动](../api/projectrome-delete-activity.md) | 无内容 | 从您的应用程序中删除该用户的指定活动。|
|[获取活动](../api/projectrome-get-activities.md) | [活动](projectrome-activity.md)集合 | 获取适用于给定用户的应用程序活动。|
|[获取最近的活动](../api/projectrome-get-recent-activities.md) | [活动](projectrome-activity.md)集合 | 为给定用户获取应用程序最近的活动, 并根据最近创建或更新的[historyItems](projectrome-historyitem.md)对其进行排序。|

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|userTimezone | String | 可选。 用于生成活动的用户设备所在的时区位于活动创建时;作为 Olson Id 提供的值, 以便支持跨平台表示形式。|
|createdDateTime | DateTimeOffset | 由服务器进行设置。 在服务器上创建对象时的 UTC 时间 (UTC)。 |
|lastModifiedDateTime | DateTimeOffset | 由服务器进行设置。 在服务器上修改对象时的 UTC 时间 (UTC)。 |
|id | 字符串 | 用于 URL 寻址的服务器生成的 ID。|
|appActivityId | String | 必需。 由呼叫者提供的应用程序上下文中的唯一活动 ID, 之后是不可变的。|
|activitySourceHost | String | 必需。 表示应用程序的跨平台标识映射的域的 URL。 映射存储为托管在域中或通过 Windows 开发人员中心配置的 JSON 文件。 JSON 文件命名为跨平台-应用标识符, 并在您的 HTTPS 域的根目录 (位于顶级域或包含子域) 中托管。 例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。 您必须具有每个跨平台应用程序标识的唯一文件和域 (或子域)。 例如, Word 与 PowerPoint 需要一个单独的文件和域。|
|appDisplayName | String | 可选。 用于生成活动的应用程序的简短文本说明, 在用户的本地设备上未安装应用程序时用于生成活动的情况。|
|activationUrl | String | 必需。 用于在由 appId 表示的最佳本机体验中启动活动的 URL。 如果不存在本机应用程序, 则可能启动基于 web 的应用程序。|
|fallbackUrl | String | 可选。 用于在基于 web 的应用程序中启动活动的 URL (如果有)。|
|contentUrl | String | 可选。 在事件中使用可在本机或基于 web 的应用程序体验之外呈现 (例如, 指向 RSS 源中的项的指针)。|
|visualElements| [visualInfo](../resources/projectrome-visualinfo.md) | 必需。 包含用于在 UX 中呈现活动的信息的对象。|
|contentInfo | 非类型化 JSON 对象 | 可选。 根据[schema.org](https://schema.org)语法的内容的自定义数据 JSON-LD 可扩展说明。|
|expirationDateTime | DateTimeOffset | 由服务器进行设置。 当对象在服务器上过期时的日期时间 (UTC)。|
|status | status | 由服务器进行设置。 用于标识有效对象的状态代码。 值: 活动、已更新、已删除、已忽略。|

## <a name="relationships"></a>关系

|关系 | 类型 | 说明|
|:------------|:-----|:-----------|
|historyItems| [activityHistoryItem](../resources/projectrome-historyitem.md)集合 | 可选。 NavigationProperty/包含;指向活动的 historyItems 的导航属性。|

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
