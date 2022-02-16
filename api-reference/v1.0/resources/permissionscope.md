---
title: permissionScope 资源类型
description: 表示委派权限的定义，有时称为 OAuth 2.0 权限或 OAuth 2.0 范围。 定义后，客户端应用程序可能会请求委派权限
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 6a3c8090ebde350a9fef944813d8754617a09c24
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854243"
---
# <a name="permissionscope-resource-type"></a>permissionScope 资源类型

命名空间：microsoft.graph

表示委派权限 [的定义](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。

委派权限可以通过需要访问令牌的客户端应用程序请求，该 API 定义了权限。 可通过 [](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)应用程序`scopes`对象的 **requiredResourceAccess** 集合，使用对 Microsoft 标识平台 的授权请求中的 参数动态请求委派权限，或静态 [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)[请求](application.md)委派权限。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|adminConsentDescription|String|委派权限的说明，供代表所有用户授予权限的管理员读取。 此文本显示在租户范围的管理员同意体验中。|
|adminConsentDisplayName|String|权限的标题，供代表所有用户授予权限的管理员读取。|
|id|GUID|为资源应用程序定义的委派权限集合中的唯一委派权限标识符。|
|isEnabled|Boolean|创建或更新权限时，必须将此属性设置为 **true** (这是默认) 。 若要删除权限，必须先将此属性设置为 **false**。  此时，在后续调用中，可能会删除权限。|
|type|String|可能的值是： `User` 和 `Admin`。 指定对于代表自己同意的非管理员用户来说，此委派权限是否安全，或者是否应该始终需要管理员同意。 虽然 Microsoft Graph为每个权限定义了默认同意要求，但租户管理员可能会通过允许、限制或限制用户对此委派权限权限授予同意来替代其组织 (中的行为) 。 有关详细信息，请参阅 [配置用户如何同意应用程序](/azure/active-directory/manage-apps/configure-user-consent)。|
|userConsentDescription|String|委派权限的说明，供代表自己授予权限的用户阅读。 此文本显示在用户仅代表自己同意的同意体验中。|
|userConsentDisplayName|String|权限的标题，供代表自己授予权限的用户读取。 此文本显示在用户仅代表自己同意的同意体验中。|
|value|String|指定要包括在访问令牌中声明 `scp` (作用域) 的值。 长度不得超过 120 个字符。 允许的字符`:` `{` `#` `$` `!` `.` `-` `,` `+` `/` `*` `)` `(` `:` `'` `&` `%` `;` <code>&lt;</code> `@` `?` `[` <code>&gt;</code> `]` `^` `_` <code>&#124;</code> `~``=` `}` `+` <code>&#96;</code>包括 、 和 范围`0-9`中的`A-Z`字符。`a-z` 不允许任何其他字符，包括空格字符。 不得以 开头 `.`。|

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
  "id": "GUID",
  "adminConsentDisplayName": "String",
  "adminConsentDescription": "String",
  "userConsentDisplayName": "String",
  "userConsentDescription": "String",
  "value": "String",
  "type": "String",
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
