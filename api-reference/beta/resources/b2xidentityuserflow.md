---
title: b2xIdentityUserFlow 资源类型
description: 表示 Azure Active Directory 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: f20e02c5f75e4133beb40315bcc4b6fc3b0712c1
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705819"
---
# <a name="b2xidentityuserflow-resource-type"></a>b2xIdentityUserFlow 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory 租户内的用户流。

用户流用于在应用程序上为来宾用户提供[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)体验。 用户流定义最终用户注册时的体验，包括他们可以使用哪些[标识提供者](/azure/active-directory/external-identities/identity-providers)进行验证，以及在注册过程中收集哪些属性。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出用户流](../api/identitycontainer-list-b2xuserflows.md)|b2xIdentityUserFlow 集合|检索所有 B2X 用户流。|
|[获取用户流](../api/b2xidentityuserflow-get.md)|b2xIdentityUserFlow|检索 B2X 用户流的属性。|
|[创建用户流](../api/identitycontainer-post-b2xuserflows.md)|b2xIdentityUserFlow|新建 B2X 用户流。|
|[删除用户流](../api/b2xidentityuserflow-delete.md)|无|删除 B2X 用户流。|
|[列出标识提供者](../api/b2xidentityuserflow-list-identityproviders.md)|[identityProvider](../resources/identityProvider.md)集合 |检索 B2X 用户流中的所有标识提供者。|
|[添加标识提供者](../api/b2xidentityuserflow-post-identityproviders.md)|无|向 B2X 用户流添加标识提供者。|
|[删除标识提供者](../api/b2xidentityuserflow-delete-identityproviders.md)|无|从 B2X 用户流中删除标识提供者。|
|[列出用户属性作业](../api/b2xidentityuserflow-list-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合|从 B2C 用户流中检索所有用户属性作业。|
|[创建用户属性作业](../api/b2xidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|在 B2C 用户流中创建一个用户属性作业。|
|[列表语言](../api/b2xidentityuserflow-list-languages.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 集合|检索 B2X 用户流中的所有语言。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|用户流名称。 这是一个必需的值且在创建之后不可变。 创建后，该名称将以 `B2X_1_` 的值作为前缀。|
|userFlowType|userFlowType|用户流类型。 对于自助注册用户流，该值在创建后只能 `signUpOrSignIn`，不能修改。|
|userFlowTypeVersion|单一|用户流版本。 对于 B2X 用户流，版本始终是`1`|

## <a name="relationships"></a>关系

| 关系       | 类型  |说明|
|:---------------|:--------|:----------|
|identityProviders|[identityProvider](../resources/identityprovider.md)集合 |用户流中包含的标识提供者。|
|userAttributeAssignments|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合|包含在用户流内的用户属性作业。|
|languages|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 集合|用户流中的自定义项所支持语言。 默认情况下，将在 B2X 用户流中启用语言自定义项。 无法在 B2X 用户流中创建自定义语言。|

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}],
    "languages": [{"@odata.type": "microsoft.graph.userFlowLanguageConfiguration"}]
}
```
