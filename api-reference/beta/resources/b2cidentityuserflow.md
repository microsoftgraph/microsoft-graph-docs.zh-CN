---
title: b2cIdentityUserFlow 资源类型
description: 表示 Azure Active Directory B2C 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 61c3a206ee07eb7e8474e501f9064a20c6cc3840
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581087"
---
# <a name="b2cidentityuserflow-resource-type"></a>b2cIdentityUserFlow 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory B2C 租户内的用户流。

为帮助你为应用程序设置最常见的标识任务，Azure Active Directory B2C 包含预定义的、可配置的策略，称为[用户流](/azure/active-directory-b2c/user-flow-overview)。 用户流可用于确定用户在执行登录、注册、编辑配置文件或重置密码等操作时与应用程序交互的方式。 可在租户中创建许多不同类型的用户流，并根据需要在应用程序中使用它们。 可以使用用户流控制以下功能：

- 用于登录的帐户类型，如 Facebook 或本地帐户等社交帐户
- 从消费者处收集的属性，例如姓名、邮政编码和鞋码
- Azure Multi-Factor Authentication
- 自定义用户界面
- 应用程序在令牌中接收的信息

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出用户流](../api/identitycontainer-list-b2cuserflows.md)|b2cIdentityUserFlow 集合|检索所 B2C 有用户流。|
|[获取用户流](../api/b2cidentityuserflow-get.md)|b2cIdentityUserFlow|检索 B2C 用户流的属性。|
|[创建用户流](../api/identitycontainer-post-b2cuserflows.md)|b2cIdentityUserFlow|新建 B2C 用户流。|
|[删除用户流](../api/b2cidentityuserflow-delete.md)|无|删除 B2C 用户流。|
|[列出标识提供者](../api/b2cidentityuserflow-list-identityproviders.md)|[identityProvider](../resources/identityProvider.md)集合 |检索 B2C 用户流中的所有标识提供者。|
|[添加标识提供者](../api/b2cidentityuserflow-post-identityproviders.md)|无|向 B2C 用户流添加标识提供者。|
|[删除标识提供者](../api/b2cidentityuserflow-delete-identityproviders.md)|无|从 B2C 用户流中删除标识提供者。|
|[列表用户属性作业](../api/b2cidentityuserflow-list-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合|从 B2C 用户流中检索所有用户属性作业。|
|[创建用户属性作业](../api/b2cidentityuserflow-post-userattributeassignments.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|在 B2C 用户流中创建所有用户属性作业。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|用户流名称。 这是一个必需的值且在创建之后不可变。 创建后，该名称将以 `B2C_1_` 的值作为前缀。|
|userFlowType|字符串|[用户流类型](/azure/active-directory-b2c/user-flow-versions)。 **userFlowType** 支持的值有：<br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|userFlowTypeVersion|单一|用户流版本。|

## <a name="relationships"></a>关系

| 关系       | 类型  |说明|
|:---------------|:--------|:----------|
|identityProviders|[identityProvider](../resources/identityprovider.md)集合 |用户流中包含的标识提供者。|
|userAttributeAssignments|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合|包含在用户流内的用户属性作业。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
  "optionalProperties": [],
  "keyProperty": "id"
} -->

```json
{
    "id": "String (identifier)",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single",
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}]
}
```
