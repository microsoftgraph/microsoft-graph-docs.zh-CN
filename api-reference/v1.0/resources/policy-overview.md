---
title: 策略 API 概述
description: Azure Active Directory策略来控制贵组织的 Azure AD 功能行为。
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: f707e34fd0db7e37efecb03883e512e367192a2b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098501"
---
# <a name="azure-ad-policy-overview"></a>Azure AD 策略概述

命名空间：microsoft.graph

Azure Active Directory (Azure AD) 使用策略来控制组织中 Azure AD 功能的行为。 策略是可针对应用程序、服务主体、组或分配到的整个组织强制执行的自定义规则。

## <a name="what-policies-are-available"></a>哪些策略可用？

| 策略类型       | 说明 | 示例 |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| 表示一个策略，该策略控制在一段时间不活动后对支持基于活动的超时功能的应用程序自动注销 Web 会话。| 将 Azure 门户配置为不活动超时 15 分钟。 |
|[authenticationFlowsPolicies](authenticationflowspolicy.md)| 表示控制外部用户是否应该能够通过外部标识自助注册用户流注册和获取来宾帐户的策略。| 使应用程序支持外部用户通过自助注册用户流进行注册。 |
|[claimsMappingPolicies](claimsMappingPolicy.md)| 表示 WS-Fed、SAML、OAuth 2.0 和 OpenID 连接协议（针对颁发给特定应用程序的令牌）声明映射策略。 | 创建并分配策略以省略颁发给服务主体的令牌中的基本声明。 |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| 表示用于控制联盟Azure Active Directory身份验证行为的策略，特别是针对联合域中的自动加速和用户身份验证限制。| 将所有用户配置为跳过主页领域发现并直接路由到 ADFS 进行身份验证。 |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|表示用于访问受保护资源的访问令牌的生存期持续时间。| 将特别敏感的应用程序配置为比默认令牌生存期更短的应用程序。|
|[tokenIssuancePolicy](tokenIssuancePolicy.md)|表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。| 配置要用于颁发 SAML 令牌的签名算法或 SAML 令牌版本。
|[identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)|表示 Azure AD 安全默认值策略。| 配置 Azure AD 安全默认策略，以抵御常见攻击。

## <a name="next-steps"></a>后续步骤

* 查看上面列出的不同策略方法及其各种方法。
* 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。
