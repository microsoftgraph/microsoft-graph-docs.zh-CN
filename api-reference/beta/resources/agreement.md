---
title: 协议资源类型
description: 表示租户的可自定义使用条款协议，它是使用 Azure Active Directory （Azure AD）创建和管理的。 您可以根据您的方案使用以下方法来创建和管理 Azure Active Directory 使用条款功能。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d698aa85f38061ce22d63f37ea3deca3635ba219
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870951"
---
# <a name="agreement-resource-type"></a>协议资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的可自定义使用条款协议，它是使用 Azure Active Directory （Azure AD）创建和管理的。 您可以根据您的方案使用以下方法来创建和管理[Azure Active Directory 使用条款功能](/azure/active-directory/active-directory-tou)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建协议](../api/agreement-post-agreements.md) | [本](agreement.md) | 通过发布到协议集合创建新协议。 |
| [列出协议](../api/agreement-list.md) | [协议](agreement.md)集合 | 获取一个协议对象集合。 |
| [获取协议](../api/agreement-get.md) | [本](agreement.md) | 读取协议对象的属性和关系。 |
| [更新协议](../api/agreement-update.md) | [本](agreement.md) | 更新协议对象。 |
| [删除协议](../api/agreement-delete.md) | 无 | 删除协议对象。 |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|协议的显示名称。|
|id|String| 只读。|
|isViewingBeforeAcceptanceRequired|Boolean|指示用户是否必须在接受前展开并查看协议。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|files|[agreementFile](agreementfile.md)集合|只读。 链接到此协议的 Pdf。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
