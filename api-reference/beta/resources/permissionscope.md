---
title: permissionScope 资源类型
description: 表示委派权限（有时称为 OAuth 2.0 权限或 OAuth 2.0 作用域）的定义。 一旦定义，客户端应用程序可能会请求委派权限
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ea3205139bffa11ff8fbe67d1ab6abb426bc65ca
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406173"
---
# <a name="permissionscope-resource-type"></a>permissionScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [委派权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)的定义。

需要对定义了权限的 API 拥有访问令牌的客户端应用程序可以请求委派权限。 可以[dynamically](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)使用 `scopes` 对 Microsoft identity 平台的授权请求中的参数（或[静态](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)）通过[application](application.md)对象上的**requiredResourceAccess**集合来动态请求委派权限。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|adminConsentDescription|字符串|委派权限的说明，供管理员用来代表所有用户授予权限来阅读。 此文本显示在租户范围内的管理员同意体验中。|
|adminConsentDisplayName|字符串|权限的标题，由管理员代表授予所有用户的权限来读取。|
|id|Guid|为资源应用程序定义的委派权限集合中的唯一委派权限标识符。|
|isEnabled|Boolean|在创建或更新权限时，此属性必须设置为 **true** (这是默认) 。 若要删除权限，必须首先将此属性设置为 **false**。  此时，在后续调用中，可能会删除该权限。|
|type|字符串|指定是否应将此委派权限视为非管理员用户同意代表自己同意，或者是否需要管理员同意权限才能。 这将是默认行为，但每个客户可以通过允许、限制或限制用户同意此委派权限来选择自定义其组织中的行为 (。 ) |
|userConsentDescription|字符串|委派权限的说明，用于代表自己授予权限的用户阅读。 此文本在同意体验中显示，其中用户仅代表自己。|
|userConsentDisplayName|字符串|权限的标题，旨在供代表自己授予权限的用户阅读。 此文本在同意体验中显示，其中用户仅代表自己。|
|value|String|指定要包含在 `scp` access 令牌中) 声明的 (范围中的值。 长度不得超过120个字符。 允许的字符包括 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` ，以及范围中的字符 `0-9` `A-Z` 和 `a-z` 。 不允许使用任何其他字符，包括空格字符。|

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