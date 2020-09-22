---
title: identityProvider 资源类型
description: 表示 Azure Active Directory (Azure AD) 标识提供程序。
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d8c3b9315df0e4fa4a21480f6be1ad283e43502d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086688"
---
# <a name="identityprovider-resource-type"></a>identityProvider 资源类型

命名空间：microsoft.graph

表示 Azure Active Directory (Azure AD) 标识提供程序。 标识提供程序可以是 Microsoft、Google、Facebook、Amazon、领英或 Twitter。 下列标识提供程序处于预览版状态：微博、QQ、微信、GitHub 以及 OpenID Connect 支持的所有提供程序。 

通过在 Azure AD B2C 中配置标识提供程序，使用户能够执行以下操作：

* 在使用者应用程序中通过社交帐户进行注册和登录。 例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户注册服务。
* 将现有本地帐户链接到使用者应用程序中的社交帐户。 例如，用户已在应用程序中创建用户名和密码（本地帐户）。 之后，用户决定将现有本地帐户链接到其 Facebook 帐户，以便能使用 Facebook 进行登录。

通过在 Azure AD B2C 中配置标识提供程序，可实现之后的 B2B 来宾方案。 例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。 Gmail 将使用其 Google 帐户凭据来验证和访问文档。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 identityProvider](../api/identityprovider-get.md) |identityProvider|读取现有 identityProvider 中的属性。|
|[创建 identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|新建 identityProvider。|
|[更新 identityProvider](../api/identityprovider-update.md)|无|更新现有的 identityProvider。|
|[删除 identityProvider](../api/identityprovider-delete.md)|无|删除现有的 identityProvider。|
|[列出 identityProvider](../api/identityprovider-list.md)|identityProvider 集合|列出在租户中配置的所有 identityProvider。|

## <a name="properties"></a>属性

|属性|类型|必需|可为空|说明|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|字符串|是|否|应用程序的客户端 ID。 这是向标识提供程序注册应用程序时获取的客户端 ID。|
|clientSecret|字符串|是|否|应用程序的客户端密码。 这是向标识提供程序注册应用程序时获取的客户端密码。 这是只读的。 读取操作将返回“\*\*\*\*”。|
|id|字符串|否|否|标识提供程序的 ID。|
|name|字符串|否|否|标识提供程序的显示名称。|
|type|字符串|是|否|标识提供程序类型。 它必须是 B2C 方案的下列值之一： <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>领英<li/>Facebook<li/>GitHub<li/>Twitter<li/>微博<li/>QQ<li/>微信</ul>在 B2B 方案中，该值必须是 Google 或 Facebook。|

### <a name="where-to-get-the-client-id-and-secret"></a>获取客户端 ID 和密码的位置

每个标识提供程序都有一个用于创建应用注册的进程。 例如，用户在 [developers.facebook.com](https://developers.facebook.com/) 处向 Facebook 创建一个应用注册。 生成的客户端 ID 和客户端密码可传递用于[创建 identityProvider](../api/identityprovider-post-identityproviders.md)。 然后，目录中的每个用户对象都可联合到租户的任意标识提供程序中进行身份验证。 这样，用户即可通过在标识提供程序的登录页面上输入评估凭据来进行登录。 来自标识提供程序的令牌先由 Azure AD 进行验证，然后租户再向应用程序发出一个令牌。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```

