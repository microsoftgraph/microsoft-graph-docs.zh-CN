---
title: objectIdentity 资源类型
description: 表示用于登录用户帐户的标识。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 45950595cc988698fcaf57bd2b9fcd913e5eeba3
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767459"
---
# <a name="objectidentity-resource-type"></a>objectIdentity 资源类型

命名空间：microsoft.graph

表示用于登录用户帐户的标识。 标识由 Microsoft、组织或与用户帐户绑定的社会标识提供者（如 Facebook、Google 或 Microsoft）提供。 这使用户能够使用这些关联标识中的任一标识登录用户帐户。

用户 **资源的 identities** [属性是](user.md) **objectIdentity** 对象。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|signInType|String| 指定目录中的用户登录类型，如 、 `emailAddress` `userName` 、 或 `federated` `userPrincipalName` 。 `federated` 表示颁发者中用户的唯一标识符，该标识符可以是颁发者选择的任何格式。 设置或更新 `userPrincipalName` 标识将更新 user 对象上的 **userPrincipalName** 属性的值。 在用户对象上的 属性上执行的验证（例如，验证域和可接受的字符）将在设置或更新标识时 `userPrincipalName` `userPrincipalName` 执行。 当登录类型设置为 或 时， **对 issuerAssignedId** 强制执行其他 `emailAddress` 验证 `userName` 。 此属性还可以设置为任何自定义字符串。 |
|issuer|string|指定标识的颁发者，例如 `facebook.com` 。<br>对于未 (**signInType** 的本地帐户) ，此属性是本地 `federated` B2C 租户的默认域名，例如 `contoso.onmicrosoft.com` 。<br>对于来自其他 Azure AD 组织的外部用户，这将是联盟组织的域，例如 `contoso.com` 。<br><br>支持 `$filter`。 512 个字符限制。|
|issuerAssignedId|string|指定颁发者分配给用户的唯一标识符。 颁发者 **与** **issuerAssignedId** 的组合在组织中必须是唯一的。 表示用户的登录名，当 **signInType** 设置为 或 (也称为本地帐户 `emailAddress` `userName`) 。<br>当 **signInType** 设置为： <ul><li>`emailAddress`、 (或以 （如) ）开头的自定义字符串必须是 `emailAddress` `emailAddress1` 有效的电子邮件地址</li><li>`userName`**，issuerAssignedId** 必须是电子邮件地址 [的有效本地部分](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>支持 `$filter`。 100 个字符限制。|

>**注意：** 筛选 **identities** 属性时，您必须同时提供 **issuer** 和 **issuerAssignedId**。

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

