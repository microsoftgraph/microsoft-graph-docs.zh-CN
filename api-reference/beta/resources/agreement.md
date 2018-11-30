---
title: 协议资源类型
description: 表示一个租户的可自定义的创建和管理与 Azure Active Directory (Azure AD) 使用协议条款。 可以使用以下方法来创建和管理 Azure Active Directory 使用条款的功能，根据您的方案。
ms.openlocfilehash: 2e5c9087cd809f9c067150654d420fda533ca61b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043803"
---
# <a name="agreement-resource-type"></a>协议资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示一个租户的可自定义的创建和管理与 Azure Active Directory (Azure AD) 使用协议条款。 可以使用以下方法来创建和管理[Azure Active Directory 使用条款的功能](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)，根据您的方案。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建协议](../api/agreement-post-agreements.md) | [协议](agreement.md) | 通过发布到协议集合中创建新的协议。 |
| [列表协议](../api/agreement-list.md) | [协议](agreement.md)集合 | 获取协议对象集合。 |
| [获取协议](../api/agreement-get.md) | [协议](agreement.md) | 读取属性和协议对象的关系。 |
| [更新协议](../api/agreement-update.md) | [协议](agreement.md) | 更新协议对象。 |
| [删除协议](../api/agreement-delete.md) | 无 | 删除协议对象。 |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|字符串|协议中的显示名称。|
|id|String| 只读。|
|isViewingBeforeAcceptanceRequired|布尔|指示用户是否能够展开和查看接受之前协议。|

## <a name="relationships"></a>Relationships
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|files|[agreementFile](agreementfile.md)集合|只读。 Pdf 链接到此协议。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
