---
title: policyRoot 资源类型
description: 公开策略单一实例导航属性的资源类型。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d684759f79fbcf4316c97876c7ee7e11be6de2d5
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768110"
---
# <a name="policyroot-resource-type"></a>policyRoot 资源类型

命名空间：microsoft.graph

公开策略单一实例导航属性的资源类型。

## <a name="methods"></a>方法
None

## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系

| 关系                              | 类型                                                                                                      | 说明                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| accessReviewPolicy                        | [accessReviewPolicy](accessreviewpolicy.md)                                                               | 包含目录级访问评审设置的策略。                                                                                                     |
| activityBasedTimeoutPolicies              | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) 集合                                    | 用于控制应用程序的 Web 会话空闲超时的策略。                                                                                        |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | 为整个租户创建和管理同意请求的策略。                                                                                  |
| appManagementPolicies                     | [appManagementPolicy](appmanagementpolicy.md) 集合                                                  | 对特定应用程序和服务主体强制实施应用管理限制的策略，重写 defaultAppManagementPolicy。                   |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | 外部用户自助注册体验的策略配置。                                                                                   |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | 在 Azure Active Directory (Azure AD) 中，允许其登录和执行多重身份验证 (MFA) 的身份验证方法和用户。 |
| authorizationPolicy                       | [authorizationPolicy](authorizationpolicy.md) 集合                                                  | 控制 Azure AD 授权设置的策略。                                                                                                            |
| b2cAuthenticationMethodsPolicy            | [b2cAuthenticationMethodsPolicy](b2cauthenticationmethodspolicy.md)                                       | 用于定义最终用户如何通过本地帐户注册的 Azure AD B2C 策略。                                                                                     |
| claimsMappingPolicies                     | [claimsMappingPolicy](claimsmappingpolicy.md) 集合                                                  | WS-Fed、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射策略，用于颁发给特定应用程序的令牌。                                   |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | 定义访问方案的自定义规则。                                                                                                                     |
| crossTenantAccessPolicy                   | [crossTenantAccessPolicy](crosstenantaccesspolicy.md)                           | 定义与外部 Azure AD 租户交互时的访问方案的自定义规则。                                                                                                                     |
| defaultAppManagementPolicy                | [tenantAppManagementPolicy](tenantappmanagementpolicy.md)                                                 | 对所有应用程序和服务主体强制实施应用管理限制的租户范围策略。                                                        |
| externalIdentitiesPolicy                  | [externalIdentitiesPolicy](externalidentitiespolicy.md)                                                   | 表示租户范围的策略，该策略控制外部用户是否可以通过自助式控制离开 Azure AD 租户。 |
| featureRolloutPolicies                    | [featureRolloutPolicy](featurerolloutpolicy.md) 集合                                                | 与目录对象关联的功能推出策略。                                                                                                       |
| homeRealmDiscoveryPolicies                | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合                                        | 用于控制联合用户的 Azure AD 身份验证行为的策略。                                                                                          |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | 表示可防范常见攻击的安全默认值的策略。                                                                                |
| mobileAppManagementPolicies               | [mobilityManagementPolicy](mobilitymanagementpolicy.md) 集合                                        | 为移动管理 (MDM 或 MAM) 应用程序定义自动注册配置的策略。                                                            |
| permissionGrantPolicies                   | [permissionGrantPolicy](permissiongrantpolicy.md) 集合                                              | 指定可以授予许可的条件的策略。                                                                                         |
| roleManagementPolicies                    | [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合                     | 表示角色管理策略。                                                                                                                             |
| roleManagementPolicyAssignments           | [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 集合 | 表示角色管理策略分配。                                                                                                                   |
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
  "@odata.type": "#microsoft.graph.policyRoot"
}
```
