---
title: homeRealmDiscoveryPolicy 资源类型
description: 表示用于控制联盟Azure Active Directory身份验证行为的策略。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 10142d22b37af4e1cff26e65c4325def6d7faefd96e2f66e56b9d5cd68acf0f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230716"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>homeRealmDiscoveryPolicy 资源类型

命名空间：microsoft.graph

表示用于控制联盟Azure Active Directory身份验证行为的策略，特别是针对联合域中的自动加速和用户身份验证限制。 您可以为组织的所有服务主体或组织中特定的服务主体设置 **homeRealmDiscoveryPolicy。** 有关更多方案和策略详细信息，请参阅使用家庭领域发现策略为应用程序配置[Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal)登录行为，以及使用电子邮件作为备用登录[ID](/azure/active-directory/authentication/howto-authentication-use-email-signin)Azure Active Directory登录。

继承自 [stsPolicy](stsPolicy.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-list.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | 读取 homeRealmDiscoveryPolicies 对象的属性和关系。 |
| [创建 homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | 创建 homeRealmDiscoveryPolicy 对象。 |
| [获取 homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | 读取 homeRealmDiscoveryPolicy 对象的属性和关系。 |
| [更新 homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md) | 无 | 更新 homeRealmDiscoveryPolicy 对象。 |
| [删除 homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-delete.md) | 无 | 删除 homeRealmDiscoveryPolicy 对象。 |
| [List appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md) | [directoryObject](directoryobject.md) collection | 获取已应用此策略的 directoryObjects 列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 此策略的唯一标识符。 只读。|
|definition|String collection| 包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。 有关此属性的 JSON 架构的更多详细信息，请参阅下文。 必需。|
|description|String| 此策略的说明。|
|displayName|String| 此策略的显示名称。 必填。|
|isOrganizationDefault|Boolean|如果设置为 true，则激活此策略。 同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认策略。 可选，默认值为 false。|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>主领域发现策略定义的属性
下面的属性构成表示令牌生存期策略的 JSON 对象。 此 JSON 对象必须 **转换为** 转义为要插入到定义属性中的引号 **的** 字符串。 下面以 JSON 格式显示了一个示例：

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\",
      \"AlternateIdLogin\":{\"Enabled\":true}}}"
  ]
```

| 属性     | 类型   |说明| 
|:---------------|:--------|:----------|
|AccelerateToFederatedDomain|Boolean| 设置为" `true` 自动加速"， (主领域发现) 。 如果租户中只有一个已验证和联合域，用户将直接进入联合身份提供程序 (如 `true` ADFS) 登录。 如果 `true` 租户中存在多个已验证域，则必须指定 **PreferredDomain。** 可选。|
|PreferredDomain|String| 指定加速登录的域。 如果租户只有一个联盟域，可以省略它。 如果省略它，并且存在多个已验证的联合域，则此策略不起作用。 如果 **AccelerateToFederatedDomain** 为 ，则必需 `true` 。|
|AllowCloudPasswordValidation|Boolean| 设置为 以允许应用程序通过直接向令牌终结点呈现用户名/密码凭据来Azure Active Directory `true` 用户。 仅在启用密码哈希同步时有效。 可选。|
|AlternateIdLogin| Json |设置为 {"Enabled"： true} 以允许 Azure AD 使用电子邮件作为 [备用登录 ID 登录](/azure/active-directory/authentication/howto-authentication-use-email-signin)。 仅在 **IsOrganizationDefault** 设置为 时有效 `true` 。 可选。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) collection| 已应用此策略的 [directoryObject](directoryObject.md) 集合。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "homeRealmDiscoveryPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
