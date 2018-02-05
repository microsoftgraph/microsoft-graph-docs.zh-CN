---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 0f5afaeff29da6f3a6330975adece44731e014bc
ms.sourcegitcommit: 4bdff5fdaea824c7c1204ec7dd641abc282d32a1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2018
---
# <a name="listitem-resource"></a>ListItem 资源

此资源表示 SharePoint **[list][]** 中的项目。
该列表中的列值可通过 `fieldValueSet` 字典获得。

## <a name="tasks-on-a-listitem"></a>listItem 上的任务

下列任务可用于 **listItem** 资源。
下面的所有示例都与**[列表][]**相关，例如：`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`。

| 常见任务                    | HTTP 方法
|:-------------------------------|:------------------------
| [获取][]                        | GET /items/{item-id}
| [获取列值][Get]       | GET /items/{item-id}?expand=fields
| [创建][]                     | POST /items
| [删除][]                     | DELETE /items/{item-id}
| [更新][]                     | PATCH /items/{item-id}
| [更新列值][Update] | PATCH /items/{item-id}/fields

[获取]: ../api/listItem_get.md
[创建]: ../api/listItem_create.md
[删除]: ../api/listItem_delete.md
[更新]: ../api/listItem_update.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **listItem** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

**listItem** 资源具有以下属性。

| 属性名称 | 类型                | 说明
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | 此列表项的内容类型
| fields        | [fieldValueSet][]   | 在此列表项上设置的列的值。

以下属性继承自 ** [baseItem][]**。

| 属性名称        | 类型             | 说明
|:---------------------|:-----------------|:-----------------------------------
| id                   | string           | 项的唯一标识符。只读。
| name                 | string           | 项目名称/标题。
| createdBy            | [identitySet][]  | 此项的创建者的标识。 只读。
| createdDateTime      | DateTimeOffset   | 创建项目的日期和时间。只读。
| 说明          | string           | 项目的描述性文本。
| lastModifiedBy       | [identitySet][]  | 此项的最后一个修饰符的标识。 只读。
| lastModifiedDateTime | DateTimeOffset   | 上次修改项目的日期和时间。只读。
| WebUrl               | string (url)     | 在浏览器中显示此项目的 URL。只读。

## <a name="relationships"></a>关系

 **listItem** 资源与其他资源具有以下关系。

| 关系名称 | 类型                        | 说明
|:------------------|:----------------------------|:-------------------------------
| driveItem         | [driveItem][]               | 对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
