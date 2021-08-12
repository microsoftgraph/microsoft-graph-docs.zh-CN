---
title: profilePhoto 资源类型
description: 从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1733a1cc102257345b609b34d40f44d972393cbacc37e321eac437b1a6da734b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163696"
---
# <a name="profilephoto-resource-type"></a>profilePhoto 资源类型

命名空间：microsoft.graph

从 Exchange Online 访问的用户、组或 Outlook 联系人的个人资料照片。它是不以 base-64 编码的二进制数据。

Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 profilePhoto](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |获取指定的 **profilePhoto** 或其元数据（profilePhoto 属性）。|
|[更新](../api/profilephoto-update.md) | [profilePhoto](profilephoto.md)  |将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|只读。|
|height|int32|照片的高度。只读。|
|width|int32|照片的宽度。只读。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

