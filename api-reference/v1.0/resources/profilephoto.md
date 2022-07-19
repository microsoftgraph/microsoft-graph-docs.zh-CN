---
title: profilePhoto 资源类型
description: 重复从 Exchange Online 或 Azure Active Directory (Azure AD) 访问的用户、组、团队或 Outlook 联系人的配置文件照片。
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7a149d1321766298b6d55977ce58b2601c4c88cf
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856118"
---
# <a name="profilephoto-resource-type"></a>profilePhoto 资源类型

命名空间：microsoft.graph

重复从 Exchange Online 或 Azure Active Directory (Azure AD) 访问的用户、组、团队或 Outlook 联系人的配置文件照片。 数据是二进制数据，而不是在 base-64 中进行编码。

Exchange Online支持高清照片的大小如下所示：`48x48`、、、`96x96`、`240x240``120x120`、`432x432``360x360`、和`504x504``648x648`。 `64x64` 在 Azure AD 中，照片可以是任何维度。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|读取个人资料照片对象的属性和关系。|
|[更新 profilePhoto](../api/profilephoto-update.md)|[profilePhoto](../resources/profilephoto.md)|更新配置文件照片对象的属性。|

> [!NOTE]
> Azure AD B2C 租户目前不支持使用 Microsoft 图形 API管理用户的照片。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|只读。|
|height|int32|照片的高度。只读。|
|width|int32|照片的宽度。只读。|

## <a name="relationships"></a>关系
无。


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
  "id": "String",
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

