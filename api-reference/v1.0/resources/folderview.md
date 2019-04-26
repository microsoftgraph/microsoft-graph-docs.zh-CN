---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 01b9860284f87ea31a969055fe2bfc7da624d3b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564111"
---
# <a name="folderview-resource-type"></a>FolderView 资源类型

**FolderView** 资源提供或设置关于文件夹的用户体验建议。

可通过 [driveItem][item-resource] 资源的 [folder][folder-facet] 属性获取。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a>属性

| 属性名称         | 类型   | 说明
|:----------------------|:-------|:--------------------------------------------
| **sortBy**            | string | 文件夹应采用的排序方法。
| **sortOrder**         | string | 如果为 true，表明应按降序排列项。 否则，应按升序排列项。
| **viewType**          | string | 应用于表示文件夹的视图类型。

可以使用 _sortBy_ 属性控制遵循 **viewType** Facet 的应用中项的排序顺序。

### <a name="sortby-options"></a>sortBy 选项

以下值是针对 **sortBy** 属性进行定义。

| 值                    | 说明
| ------------------------ | --------------------------------------------------
| `default`                | 应用的默认排序顺序。
| `name`                   | 应按项的 **name** 属性排列项。
| `type`                   | 应按项类型排列项。
| `size`                   | 应按项的 **size** 属性排列项。
| `takenOrCreatedDateTime` | 应按 **Photo** Facet 的 **takenDateTime** 属性排列项。 如果此属性不可用，应按 **createdDateTime** 属性排列项。
| `lastModifiedDateTime`   | 应按项的 **lastModifiedDateTime** 属性排列项。
| `sequence`               | 这些项按照用户指定的自定义序列排列。


### <a name="sortorder-options"></a>sortOrder 选项

以下值是针对 **sortOrder** 属性进行定义。

| 值        | 说明
| ------------ | --------------------------------------------------------------
| `ascending`  | 应按升序排列项。
| `descending` | 应按降序排列项。


### <a name="viewtype-options"></a>viewType 选项

以下值是针对 **viewType** 属性进行定义。

| 值        | 说明
| ------------ | --------------------------------------------------------------
| `default`    | 应用的默认视图类型。
| `icons`      | 使用图标表示 driveItem 的视图。
| `details`    | 使用多个列提供每一项的其他详细信息的视图。
| `thumbnails` | 使用 driveItem 的大缩略图表示项的视图。


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,icons,details,thumbnails) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,name,type,size,takenOrCreatedDateTime,lastModifiedDateTime,sequence) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(ascending,descending) are in resource, but () are in table"
  ],
  "tocPath": "Facets/FolderView"
} -->
