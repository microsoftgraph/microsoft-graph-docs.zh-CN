---
title: objectIdentity 资源类型
description: 表示用于登录到用户帐户的标识。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 93c7fb05945e9924c95031fb8392443acdd0a1ae
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095088"
---
# <a name="objectidentity-resource-type"></a>objectIdentity 资源类型

命名空间：microsoft.graph

表示用于登录到用户帐户的标识。 Microsoft、组织或与用户帐户相关联的社交标识提供者（如 Facebook、Google 或 Microsoft）可以提供标识。 这样，用户就可以使用这些关联标识登录到用户帐户。

[用户](user.md)资源的标 **识** 属性是 **objectIdentity** 对象。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|signInType|String| 指定目录中的用户登录类型，例如`emailAddress`，`userName``federated``userPrincipalName`或 。 `federated` 表示颁发者中用户的唯一标识符，该标识符可以采用颁发者选择的任何格式。 设置或更新标 `userPrincipalName` 识将更新用户对象上的 **userPrincipalName** 属性的值。 在 `userPrincipalName` 设置或更新 `userPrincipalName` 标识时，将对用户对象上的属性执行验证，例如已验证的域和可接受的字符。 当登录类型设置为`emailAddress`或`userName`设置时，在 **issuerAssignedId** 上强制执行其他验证。 此属性还可以设置为任何自定义字符串。 |
|发行|string|指定标识的颁发者，例如 `facebook.com`。<br>例如，对于不`federated`) **signInType** (本地帐户，`contoso.onmicrosoft.com`此属性是本地 B2C 租户默认域名。<br>例如，对于来自其他 Azure AD 组织的外部用户， `contoso.com`这将是联合组织的域。<br><br>支持 `$filter`。 512 个字符限制。|
|issuerAssignedId|string|指定颁发者分配给用户的唯一标识符。 **颁发者** 与 **issuerAssignedId** 的组合在组织中必须是唯一的。 表示在 **将 signInType** 设置 `emailAddress` 为或 `userName` (也称为本地帐户) 时用户的登录名称。<br>将 **signInType** 设置为： <ul><li>`emailAddress`、 (或自定义字符串（ `emailAddress` 以) `emailAddress1` **issuerAssignedId** 开头）必须是有效的电子邮件地址</li><li>`userName`， **issuerAssignedId** 必须是 [电子邮件地址的有效本地部分](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>支持 `$filter`。 100 个字符限制。|

### <a name="filtering"></a>筛选
筛选 **issuerAssignedId** 的 **标识** 属性时，必须同时提供 **颁发者** 和 **issuerAssignedId**。 此外：
- 筛选具有 **signInType** 的 `federated` 条目需要有效的 **颁发者** 和 **颁发者AssignedId**。
- 筛选具有 **signInType** 或`emailAddress`忽略颁发者值的`userName`条目。 这是设计使然的。 
- 不支持筛选具有 **signInType** 的 `userPrincipalName` 条目。 这可以通过筛选用户对象上的 **userPrincipalName** 属性来实现。

以下值仅支持对 **颁发者** 进行筛选：`google.com`、`facebook.com`和 `mail``phone`。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectIdentity"
}-->

```json
{
  "signInType": "string",
  "issuer": "string",
  "issuerAssignedId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

