---
title: b2xUserFlows 资源类型
description: 表示 Azure Active Directory 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 989fbb3e003acd4207740a300c1b6f5d0c926e08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089747"
---
# <a name="b2xuserflows-resource-type"></a>b2xUserFlows 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory 租户内的用户流。

用户流用于在应用程序上为来宾用户提供[自助注册](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview)体验。 用户流定义最终用户注册时的体验，包括他们可以使用哪些[标识提供者](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers)进行验证，以及在注册过程中收集哪些属性。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出用户流](../api/b2xuserflows-list.md)|b2xUserFlow 集合|检索所有用户流。|
|[获取用户流](../api/b2xuserflows-get.md)|b2xUserFlow|检索用户流的属性。|
|[创建用户流](../api/b2xuserflow-post-b2xuserflows.md)|b2xUserFlow|新建用户流。|
|[删除用户流](../api/b2xuserflows-delete.md)|无|删除用户流。|
|[列出标识提供者](../api/b2xuserflows-list-identityproviders.md)|[identityProvider](../resources/identityProvider.md)集合 |检索用户流中的所有标识提供者。|
|[添加标识提供者](../api/b2xuserflows-update-identityprovider.md)|无|向用户流添加标识提供者。|
|[删除标识提供者](../api/b2xuserflows-delete-identityprovider.md)|无|从用户流中删除标识提供者。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|用户流名称。 这是一个必需的值且在创建之后不可变。 创建后，该名称将以 `B2X_1_` 的值作为前缀。|
|userFlowType|字符串|用户流类型。 对于自助注册用户流，该值在创建后只能 `signUpOrSignIn`，不能修改。|
|userFlowVersion|单一|用户流版本。 对于 B2X 用户流，版本始终是`1`|

## <a name="relationships"></a>关系

| 关系       | 类型  |说明|
|:---------------|:--------|:----------|
|identityProviders|[identityProvider](../resources/identityprovider.md)集合 |用户流中包含的标识提供者。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "optionalProperties": [],
  "keyProperty": "id"
} -->

```json
{
    "id": "String (identifier)",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single",
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```


