---
title: policyRoot 资源类型
description: 公开策略单一元素的导航属性的资源类型。
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6f0a5b9862a955b9508fb9a9075a848646dbcac8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688435"
---
# <a name="policyroot-resource-type"></a>policyRoot 资源类型

命名空间：microsoft.graph

公开策略单一元素的导航属性的资源类型。

## <a name="methods"></a>Methods
无

## <a name="properties"></a>属性
无


## <a name="relationships"></a>关系
| 关系                              | 类型                                                                                                      | 说明                                                                                                                                                             |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| accessReviewPolicy                        | [accessReviewPolicy](accessreviewpolicy.md)                                                               | 包含目录级别访问评审设置的策略。                                                                                                        |
| activityBasedTimeoutPolicies              | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) 集合                                    | 控制应用程序的 Web 会话的空闲时间的策略。                                                                                           |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | 创建和管理整个租户的同意请求的策略。                                                                                     |
| appManagementPolicies                     | [appManagementPolicy](appmanagementpolicy.md) 集合                                                  | 对特定应用程序和服务主体强制执行应用管理限制的策略，覆盖 defaultAppManagementPolicy。                      |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | 外部用户的自助注册体验的策略配置。                                                                                      |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | 身份验证方法以及允许使用它们登录并执行 MFA 中 MFA (多重) 用户Azure Active Directory (Azure AD) 。    |
| authorizationPolicy                       | [authorizationPolicy](authorizationpolicy.md) 集合                                                  | 控制授权Azure AD策略。                                                                                                               |
| b2cAuthenticationMethodsPolicy            | [b2cAuthenticationMethodsPolicy](b2cauthenticationmethodspolicy.md)                                       | 定义Azure AD帐户注册方式的 B2C 策略。                                                                                        |
| claimsMappingPolicies                     | [claimsMappingPolicy](claimsmappingpolicy.md) 集合                                                  | WS-Fed、SAML、OAuth 2.0 和 OpenID 连接协议声明映射策略，用于颁发给特定应用程序的令牌。                                      |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | 定义访问方案的自定义规则。                                                                                                                        |
| defaultAppManagementPolicy                | [tenantAppManagementPolicy](tenantappmanagementpolicy.md)                                                 | 用于强制执行所有应用程序和服务主体的应用管理限制的租户范围策略。                                                           |
| deviceRegistrationPolicy                  | [deviceRegistrationPolicy](deviceregistrationpolicy.md)                                                   | 表示控制配额限制、其他身份验证和授权策略的策略范围，以向组织注册设备标识。 |
| featureRolloutPolicies                    | [featureRolloutPolicy](featurerolloutpolicy.md) 集合                                                | 与目录对象关联的功能推出策略。                                                                                                          |
| homeRealmDiscoveryPolicies                | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合                                        | 用于控制联盟Azure AD身份验证行为的策略。                                                                                             |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | 表示用于防范常见攻击的安全默认值的策略。                                                                                   |
| mobileAppManagementPolicies               | [mobilityManagementPolicy](mobilitymanagementpolicy.md) 集合                                        | 定义移动管理自动注册配置的策略 (MDM 或 MAM) 应用程序。                                                               |
| permissionGrantPolicies                   | [permissionGrantPolicy](permissiongrantpolicy.md) 集合                                              | 指定可授予同意的条件的策略。                                                                                            |
| roleManagementPolicies                    | [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合                     | 表示角色管理策略。                                                                                                                                |
| roleManagementPolicyAssignments           | [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合 | 表示角色管理策略分配。                                                                                                                      |
| tokenIssuancePolicies                     | [tokenIssuancePolicy](tokenissuancepolicy.md) 集合                                                  | 指定由 SAML 令牌颁发者颁发的 SAML 令牌Azure AD。                                                                                        |
| tokenLifetimePolicies                     | [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合                                                  | 控制 JWT 访问令牌、ID 令牌或由应用程序颁发的 SAML 1.1/2.0 令牌的生命周期Azure AD。                                                   |

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
  "@odata.type": "#microsoft.graph.policyRoot"
}
```

