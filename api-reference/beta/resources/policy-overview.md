---
title: 策略 API 概述
description: Azure Active Directory 使用策略来控制组织中 Azure AD 功能的行为。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 39e45d28491ace2502aa8f1df0df9af0273c54da
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132645"
---
# <a name="azure-ad-policy-overview"></a>Azure AD 策略概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 使用策略来控制你的组织中 Azure AD 功能行为。 策略是可以在应用程序、服务主体、组或分配给其的整个组织上强制执行的自定义规则。

## <a name="what-policies-are-available"></a>哪些策略可用？

| 策略类型       | 说明 | 示例 |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| 表示一个策略，该策略控制支持基于活动的超时功能的应用程序在一段时间不活动后自动注销 Web 会话。| 将 Azure 门户配置为不活动超时 15 分钟。 |
|[authorizationPolicy](authorizationpolicy.md)| 表示可以控制 Azure Active Directory 的授权设置的策略。 | 配置 Azure AD 以阻止租户中的 MSOL PowerShell。 |
|[claimsMappingPolicies](claimsMappingPolicy.md)| 表示 WS-Fed、SAML、OAuth 2.0 和 OpenID Connect 协议声明映射策略，用于颁发给特定应用程序的令牌。 | 创建并分配策略以从颁发给服务主体的令牌中省略基本声明。 |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| 表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，特别是针对联合域中的自动加速和用户身份验证限制。| 将所有用户配置为跳过主领域发现，并直接路由到 ADFS 进行身份验证。 |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|表示用于访问受保护资源的访问令牌的生存期持续时间。| 将特别敏感的应用程序配置为比默认令牌生存期更短的应用程序。|
|[tokenIssuancePolicy](tokenIssuancePolicy.md)|表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。| 配置要用于颁发 SAML 令牌的签名算法或 SAML 令牌版本。
|[identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)|表示 Azure AD 安全默认策略。| 配置 Azure AD 安全默认策略，以防范常见攻击。

## <a name="next-steps"></a>后续步骤

* 查看上面列出的不同策略选择类型及其各种方法。
* 请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。


