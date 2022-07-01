---
title: policyRoot 资源类型
description: 公开策略单一实例导航属性的资源类型。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dc54d92a520961441545962fa996efd39fa8ca3d
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604480"
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
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | 在 Azure Active Directory (Azure AD) 中，允许其登录和执行多重身份验证 (MFA) 的身份验证方法和用户。 |
| authorizationPolicy                       | [authorizationPolicy](authorizationpolicy.md) 集合                                                  | 控制 Azure AD 授权设置的策略。                                                                                                            |
| claimsMappingPolicies                     | [claimsMappingPolicy](claimsmappingpolicy.md) 集合                                                  | WS-Fed、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射策略，用于颁发给特定应用程序的令牌。                                   |
| crossTenantAccessPolicy                   | [crossTenantAccessPolicy](crosstenantaccesspolicy.md)                           | 定义与外部 Azure AD 租户交互时的访问方案的自定义规则。                                                                                                                     |
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

