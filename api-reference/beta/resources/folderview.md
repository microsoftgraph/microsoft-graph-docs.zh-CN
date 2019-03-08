---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: f82242da39ebc13d769a0a3471b60dd4ac9df8dc
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480920"
---
# <a name="folderview-resource-type"></a>FolderView 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**FolderView** 资源提供或设置关于文件夹的用户体验建议。

可通过 [driveItem][item-resource] 资源的 [folder][folder-facet] 属性获取。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
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

### <a name="sortby-values"></a>sortBy 值

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


### <a name="sortorder-values"></a>sortOrder 值

以下值是针对 **sortOrder** 属性进行定义。

| 值        | 说明
| ------------ | --------------------------------------------------------------
| `ascending`  | 应按升序排列项。
| `descending` | 应按降序排列项。


### <a name="viewtype-values"></a>viewType 值

以下值是针对 **viewType** 属性进行定义。

| 值        | 说明
| ------------ | --------------------------------------------------------------
| `default`    | 应用的默认视图类型。
| `icons`      | 使用图标表示 driveItem 的视图。
| `details`    | 使用多个列提供每一项的其他详细信息的视图。
| `thumbnails` | 使用 driveItem 的大缩略图表示项的视图。


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
