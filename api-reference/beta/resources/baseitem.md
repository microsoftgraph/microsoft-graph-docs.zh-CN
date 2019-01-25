---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: 5bc3aab8460c1d0c6774d2f8afda13c4fc89f69d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521584"
---
# <a name="baseitem-resource-type"></a>BaseItem 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**baseItem** 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。从 **baseItem** 派生的资源包括：

* [drive](drive.md)
* [driveItem](driveitem.md)
* [网站](site.md)
* [sharedDriveItem](shareddriveitem.md)

## <a name="json-representation"></a>JSON 表示形式

下面是 **baseItem** 资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性             | 类型              | 说明                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| id                   | string            | 驱动器唯一标识符。只读。                                         |
| createdBy            | [identitySet][]   | 识别创建项目的用户、设备或应用程序。只读。        |
| createdDateTime      | dateTimeOffset    | 创建项的日期和时间。只读。                                             |
| eTag                 | 字符串            | 该项目的 ETag。只读。                                                          |
| lastModifiedBy       | [identitySet][]   | 上次修改项目的用户、设备和应用程序的标识。只读。 |
| lastModifiedDateTime | dateTimeOffset    | 上次修改项目的日期和时间。只读。                                   |
| name                 | string            | 项目名称。读写。                                                      |
| parentReference      | [itemReference][] | 父信息（如果此项具有父级）。读写。                              |
| WebUrl               | string (url)      | 在浏览器中显示此资源的 URL。只读。                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a>注解

`baseItem` 类型不应直接使用。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
