---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
ms.openlocfilehash: eaf73cf54671393b61cc37b5a5d1922060640882
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008867"
---
# <a name="baseitem-resource-type"></a>BaseItem 资源类型

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
  "abstract": true,
  "baseType": "microsoft.graph.entity",
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
| 说明          | 字符串            | 提供用户可见项目的说明。 可选。                             |
| eTag                 | string            | 该项目的 ETag。只读。                                                          |
| lastModifiedBy       | [identitySet][]   | 上次修改项目的用户、设备和应用程序的标识。只读。 |
| lastModifiedDateTime | dateTimeOffset    | 上次修改项目的日期和时间。只读。                                   |
| name                 | string            | 项目名称。读写。                                                      |
| parentReference      | [itemReference][] | 父信息（如果此项具有父级）。读写。                              |
| WebUrl               | string (url)      | 在浏览器中显示此资源的 URL。只读。                              |

## <a name="relationships"></a>Relationships

| 关系       | 类型     | 说明
|:-------------------|:---------|:---------------------------------------------
| createdByUser      | [用户][] | 创建了项的用户的身份。 只读。
| lastModifiedByUser | [用户][] | 上次修改项的用户的身份。 只读。

[identitySet]: identityset.md
[itemReference]: itemreference.md
[用户]: user.md

## <a name="remarks"></a>注解

`baseItem` 类型不应直接使用。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
