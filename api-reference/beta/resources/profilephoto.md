---
title: profilePhoto 资源类型
description: 从 Exchange Online 或 Azure Active Directory (AAD) 中访问的用户、组或 Outlook 联系人的个人资料照片。二进制数据未在 base-64 中进行编码。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0a9a38750cf42172a9445764e40d683e2e337600
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757245"
---
# <a name="profilephoto-resource-type"></a>profilePhoto 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从 Exchange Online 或 Azure Active Directory (AAD) 中访问的用户、组或 Outlook 联系人的个人资料照片。二进制数据未在 base-64 中进行编码。

Exchange Online 支持的 HD 照片大小如下所示：'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504' 和 '648x648'。 在 AAD 上，照片可以是任何维度。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 profilePhoto](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |获取指定的 **profilePhoto** 或其元数据（**profilePhoto** 属性）。 |
|[更新](../api/profilephoto-update.md) | [profilePhoto](profilephoto.md)  |将照片分配给指定的用户、组或联系人。照片应为二进制格式。它将替换现有的照片（如有）。 |

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

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
