---
title: 策略 API 概述
description: Azure Active Directory 使用策略来控制贵组织的 Azure AD 功能行为。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 4178a58cb0a4fae341131f89cc6047e3c7b5e4a8
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882626"
---
# <a name="azure-ad-policy-overview"></a>Azure AD 策略概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 使用策略来控制贵组织的 Azure AD 功能行为。 策略是可针对应用程序、服务主体、组或分配到的整个组织强制执行的自定义规则。

## <a name="what-policies-are-available"></a>哪些策略可用？

| 策略类型       | 说明 | 示例 |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| 表示一个策略，该策略控制在一段时间不活动后对支持基于活动的超时功能的应用程序自动注销 Web 会话。| 将 Azure 门户配置为不活动超时 15 分钟。 |
|[authenticationFlowsPolicies](authenticationflowspolicy.md)| 表示控制外部用户是否应该能够通过外部标识自助注册用户流注册和获取来宾帐户的策略。| 使应用程序支持外部用户通过自助注册用户流进行注册。 |
|[authorizationPolicy](authorizationpolicy.md)| 表示可以控制 Azure Active Directory 的授权设置的策略。 | 配置 Azure AD 以阻止租户中的 MSOL PowerShell。 |
|[claimsMappingPolicies](claimsMappingPolicy.md)| 表示 WS-Fed、SAML、OAuth 2.0 和 OpenID Connect 协议（针对颁发给特定应用程序的令牌）声明映射策略。 | 创建并分配策略以省略颁发给服务主体的令牌中的基本声明。 |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| 表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，尤其是针对联合域中的自动加速和用户身份验证限制。| 将所有用户配置为跳过主页领域发现并直接路由到 ADFS 进行身份验证。 |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|表示用于访问受保护资源的访问令牌的生存期持续时间。| 将特别敏感的应用程序配置为比默认令牌生存期更短的应用程序。|
|[tokenIssuancePolicy](tokenIssuancePolicy.md)|表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。| 配置要用于颁发 SAML 令牌的签名算法或 SAML 令牌版本。
|[identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)|表示 Azure AD 安全默认值策略。| 配置 Azure AD 安全默认策略，以抵御常见攻击。

## <a name="next-steps"></a>后续步骤

* 查看上面列出的不同策略方法及其各种方法。
* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。
