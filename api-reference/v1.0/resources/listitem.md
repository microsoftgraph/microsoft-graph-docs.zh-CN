---
author: JeremyKelley
title: listItem 资源
description: 表示 SharePoint 列表中的项目。
ms.localizationpriority: high
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 851b506b029d05bfac2bcecfcce57d9e3ce8684f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021461"
---
# <a name="listitem-resource"></a>listItem 资源

命名空间：microsoft.graph

表示 SharePoint [列表][]中的项目。

SharePoint 文档库中的所有项目可以表示为 **listItem** 或 [driveItem][] 资源。

该列表中的列值可通过 `fieldValueSet` 字典获得。

## <a name="methods"></a>方法

下列方法可用于 **listItem** 资源。
所有示例都与 **[list][]** 相关：`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`。

| 方法                    | 返回类型 | 说明
|:-------------------------------|:-------------------|:------
| [获取][]                   | listItem| 获取列表中的项。
| [获取列值][Get]       | listItem | 从 listItem 获取列的值。
| [获取分析结果][]              | [itemAnalytics][]| 对此资源可获取分析。 
| [按间隔获取活动][] | [itemActivityStat][]| 在指定的时间间隔内获取 itemActivityStats 的集合。
| [Create][]                     | listItem | 在列表中创建新的 listItem。
| [删除][]                     | 无内容 | 从 list 中删除项。
| [Update][]                     | [fieldValueSet][]| 更新 listItem 上的属性。
| [更新列值][Update] | [fieldValueSet][]| 更新 listItem 上的列值。

[Get]: ../api/listitem-get.md
[获取分析结果]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivitystat-getactivitybyinterval.md
[Create]: ../api/listitem-create.md
[删除]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a>属性

**listItem** 资源具有以下属性。

| 属性名称 | 类型                | 说明
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | 此列表项的内容类型

以下属性继承自 **[baseItem][]**。

| 属性名称        | 类型              | 说明
|:---------------------|:------------------|:----------------------------------
| id                   | string            | 项的唯一标识符。只读。
| name                 | string            | 项目名称/标题。
| createdBy            | [identitySet][]   | 此项的创建者的标识。只读。
| createdDateTime      | DateTimeOffset    | 创建项目的日期和时间。只读。
| 说明          | string            | 项目的描述性文本。
| eTag                 | 字符串            | 该项目的 ETag。只读。                                                          |
| lastModifiedBy       | [identitySet][]   | 此项最后一个修饰符的标识。只读。
| lastModifiedDateTime | DateTimeOffset    | 上次修改项目的日期和时间。只读。
| parentReference      | [itemReference][] | 父信息（如果此项具有父级）。读写。
| sharepointIds        | [sharepointIds][] | 返回对 SharePoint REST 兼容性有用的标识符。只读。
| webUrl               | string (url)      | 在浏览器中显示此项目的 URL。只读。

## <a name="relationships"></a>关系

 **listItem** 资源与其他资源具有以下关系。

| 关系名称 | 类型                           | 说明
|:------------------|:-------------------------------|:-------------------------------
| activities        | [itemActivity][] 集合    | 最近发生在此项上的活动的列表。
| 分析         | [itemAnalytics][] 资源     | 此项目上发生的查看活动的相关分析。
| driveItem         | [driveItem][]                  | 对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。
| fields            | [fieldValueSet][]              | 在此列表项上设置的列的值。
| 版本          | [listItemVersion][] 集合 | 先前版本的列表项的列表。

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **listItem** 资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl&quot;: &quot;url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/listItem",
  "tocBookmarks": {
    "ListItem&quot;: &quot;#"
  }
} -->

