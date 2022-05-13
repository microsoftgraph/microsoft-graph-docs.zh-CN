---
title: policyRoot 资源类型
description: 公开策略单一实例导航属性的资源类型。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fd9c30baa16ef404c363448f06d211613bad64e7
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398410"
---
# <a name="policyroot-resource-type"></a>policyRoot 资源类型

命名空间：microsoft.graph

公开策略单一实例导航属性的资源类型。 继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
无

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|策略的唯一标识符。 继承自 [entity](../resources/entity.md)。|


## <a name="relationships"></a>关系
| 关系                              | 类型                                                                                                      | 说明                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityBasedTimeoutPolicies              | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) 集合                                    | 用于控制应用程序的 Web 会话空闲超时的策略。                                                                                        |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | 为整个租户创建和管理同意请求的策略。                                                                                  |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | 外部用户自助注册体验的策略配置。                                                                                   |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | 允许其登录的身份验证方法和用户 (Azure AD) Azure Active Directory (中的 MFA)  (多重身份验证。 |
| authorizationPolicy                       | [authorizationPolicy](authorizationpolicy.md) 集合                                                  | 控制 Azure AD 授权设置的策略。                                                                                                            |
| claimsMappingPolicies                     | [claimsMappingPolicy](claimsmappingpolicy.md) 集合                                                  | WS-Fed、SAML、OAuth 2.0 和 OpenID 连接协议的声明映射策略，用于向特定应用程序颁发的令牌。                                   |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | 定义访问方案的自定义规则。                                                                                                                     |
| featureRolloutPolicies                    | [featureRolloutPolicy](featurerolloutpolicy.md) 集合                                                | 与目录对象关联的功能推出策略。                                                                                                       |
| homeRealmDiscoveryPolicies                | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合                                        | 用于控制联合用户的 Azure AD 身份验证行为的策略。                                                                                          |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | 表示可防范常见攻击的安全默认值的策略。                                                                                |
| permissionGrantPolicies                   | [permissionGrantPolicy](permissiongrantpolicy.md) 集合                                              | 指定可以授予许可的条件的策略。                                                                                         |
|roleManagementPolicies|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合| 指定与范围和角色关联的各种策略。 |
|roleManagementPolicyAssignments|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合| 将角色管理策略分配给角色定义对象。 |
| tokenIssuancePolicies                     | [tokenIssuancePolicy](tokenissuancepolicy.md) 集合                                                  | 指定 Azure AD 颁发的 SAML 令牌特征的策略。                                                                                     |
| tokenLifetimePolicies                     | [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合                                                  | 控制 Azure AD 颁发的 JWT 访问令牌、ID 令牌或 SAML 1.1/2.0 令牌生存期的策略。                                                |


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot",
  "id": "String (identifier)"
}
```

