---
title: permissionScope 资源类型
description: 表示委派权限的定义，有时称为 OAuth 2.0 权限或 OAuth 2.0 范围。 定义后，客户端应用程序可能会请求委派权限
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 7836685c65fddd2d35a2d9bc47493bf2f240e51653ef8a264ac868be83b02e80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196934"
---
# <a name="permissionscope-resource-type"></a>permissionScope 资源类型

命名空间：microsoft.graph

表示委派权限 [的定义](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。

委派权限可以通过需要访问令牌的客户端应用程序请求，该 API 定义了权限。 可通过 application 对象的 [](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent) `scopes` **requiredResourceAccess** 集合动态请求委派权限，使用对 Microsoft 标识平台 的授权 [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)请求中的 参数，或静态 [请求](application.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|adminConsentDescription|String|委派权限的说明，供代表所有用户授予权限的管理员读取。 此文本显示在租户范围的管理员同意体验中。|
|adminConsentDisplayName|String|权限的标题，供代表所有用户授予权限的管理员读取。|
|id|Guid|为资源应用程序定义的委派权限集合中的唯一委派权限标识符。|
|isEnabled|Boolean|创建或更新权限时，必须将此属性设置为 **true** (这是默认) 。 若要删除权限，必须先将此属性设置为 **false**。  此时，在后续调用中，可能会删除权限。|
|type|String|指定非管理员用户代表自己同意此委派权限是否安全，或者是否需要管理员同意这些权限。 这是默认行为，但每个客户都可以选择自定义其组织中的行为 (允许、限制或限制用户对此委派权限的同意。) |
|userConsentDescription|String|委派权限的说明，供代表自己授予权限的用户阅读。 此文本显示在用户仅代表自己同意的同意体验中。|
|userConsentDisplayName|String|权限的标题，供代表自己授予权限的用户读取。 此文本显示在用户仅代表自己同意的同意体验中。|
|value|String|指定要包括在访问令牌中声明 (`scp` 作用域) 的值。 长度不得超过 120 个字符。 允许的字符 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` 包括 、 和 范围 `0-9` `A-Z` 中的字符 `a-z` 。 不允许任何其他字符，包括空格字符。 不得以 开头 `.` 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "id": "guid",
  "adminConsentDisplayName": "string",
  "adminConsentDescription": "string",
  "userConsentDisplayName": "string",
  "userConsentDescription": "string",
  "value": "string",
  "type": "string",
  "isEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
