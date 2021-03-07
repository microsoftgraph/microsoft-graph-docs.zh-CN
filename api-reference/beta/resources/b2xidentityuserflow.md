---
title: b2xIdentityUserFlow 资源类型
description: 表示 Azure Active Directory 租户中的自助式注册用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 733a3b242b6c81c7ef111ccc95e9fec151e6405d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516435"
---
# <a name="b2xidentityuserflow-resource-type"></a>b2xIdentityUserFlow 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory 租户中的自助式注册用户流。

用户流用于在应用程序上为来宾用户提供[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)体验。 用户流定义最终用户注册时的体验，包括他们可以使用哪些[标识提供者](/azure/active-directory/external-identities/identity-providers)进行验证，以及在注册过程中收集哪些属性。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出用户流](../api/identitycontainer-list-b2xuserflows.md)|b2xIdentityUserFlow 集合|检索所有自助式注册用户流。|
|[获取用户流](../api/b2xidentityuserflow-get.md)|b2xIdentityUserFlow|检索自助式注册用户流的属性。|
|[创建用户流](../api/identitycontainer-post-b2xuserflows.md)|b2xIdentityUserFlow|创建新的自助式注册用户流。|
|[删除用户流](../api/b2xidentityuserflow-delete.md)|无|删除自助式注册用户流。|
|[列出标识提供者](../api/b2xidentityuserflow-list-identityproviders.md)|[identityProvider](../resources/identityProvider.md)集合 |检索自助式注册用户流中所有标识提供程序。|
|[添加标识提供者](../api/b2xidentityuserflow-post-identityproviders.md)|无|向自助式注册用户流添加标识提供程序。|
|[删除标识提供者](../api/b2xidentityuserflow-delete-identityproviders.md)|无|从自助式注册用户流中删除标识提供程序。|
|[列表用户属性作业](../api/b2xidentityuserflow-list-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合|检索自助式注册用户流中的所有用户属性分配。|
|[创建用户属性作业](../api/b2xidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|在自助式注册用户流中创建用户属性分配。|
|[列出语言](../api/b2xidentityuserflow-list-languages.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 集合|检索自助式注册用户流内的所有语言。|
|[获取用户流的 API 连接器配置](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md)|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)| 获取自助式注册用户流中使用的 API 连接器的配置。 此方法不支持 $expand 查询参数。|
|[在用户流中配置 API 连接器](../api/b2xidentityuserflow-put-apiConnectorConfiguration.md)|无| 通过更新 apiConneconfiguration 属性的 [apiConneconfiguration](../resources/userflowapiconnectorconfiguration.md) API 连接器。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|用户流名称。 这是一个必需的值且在创建之后不可变。 创建后，该名称将以 `B2X_1_` 的值作为前缀。|
|userFlowType|userFlowType|用户流类型。 对于自助注册用户流，该值在创建后只能 `signUpOrSignIn`，不能修改。|
|userFlowTypeVersion|单一|用户流版本。 对于自助式注册用户流，版本始终为 `1`。|
|apiConnectorConfiguration|[userFlowApiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)|配置，用于启用 API 连接器以作为自助式注册用户流的一部分。 只能使用 [Get userFlowApiConnectorConfiguration](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) 获取此对象的值。|

## <a name="relationships"></a>关系

| 关系       | 类型  |说明|
|:---------------|:--------|:----------|
|identityProviders|[identityProvider](../resources/identityprovider.md)集合 |用户流中包含的标识提供者。|
|userAttributeAssignments|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合|包含在用户流内的用户属性作业。|
|语言|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 集合|用户流中的支持自定义的语言。 默认情况下，自助式注册用户流中启用了语言自定义。 无法在自助式注册用户流中创建自定义语言。|

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
    "languages": [{"@odata.type": "microsoft.graph.userFlowLanguageConfiguration"}],
    "apiConnectorConfiguration": {
      "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
    }
}
```
