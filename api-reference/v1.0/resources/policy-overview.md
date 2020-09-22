---
title: 策略 API 概述
description: Azure Active Directory 使用策略控制组织中的 Azure AD 功能行为。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 189757df4313eff1ab9545b69fe5a13ed5785c9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037337"
---
# <a name="azure-ad-policy-overview"></a>Azure AD 策略概述

命名空间：microsoft.graph



Azure Active Directory (Azure AD) 使用策略控制组织中的 Azure AD 功能行为。 策略是您可以在应用程序、服务主体、组或其分配到的整个组织上实施的自定义规则。

## <a name="what-policies-are-available"></a>有哪些策略可用？

| 策略类型       | 说明 | 示例 |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| 表示在一段时间不活动后控制 web 会话的自动注销的策略，适用于支持基于活动的超时功能的应用程序。| 将 Azure 门户配置为使非活动超时为15分钟。 |
|[claimsMappingPolicies](claimsMappingPolicy.md)| 表示对颁发给特定应用程序的令牌的 WS 馈送、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射策略。 | 创建和分配策略以省略颁发给服务主体的令牌中的基本声明。 |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| 表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，尤其适用于联合域中的自动加速和用户身份验证限制。| 将所有用户配置为跳过 "主页领域发现"，并将其直接路由到 ADFS 进行身份验证。 |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|表示用于访问受保护的资源的访问令牌的生存期持续时间。| 配置一个具有短于默认令牌生存期的特别敏感的应用程序。|
|[tokenIssuancePolicy](tokenIssuancePolicy.md)|表示指定由 Azure AD 颁发的 SAML 令牌的特征的策略。| 配置用于发出 SAML 令牌的签名算法或 SAML 令牌版本。
|[identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)|代表 "Azure AD 安全性默认策略"。| 配置 Azure AD 安全性默认策略以防止受到常见攻击。

## <a name="next-steps"></a>后续步骤

* 查看上面列出的不同策略资源类型及其各种方法。
* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

