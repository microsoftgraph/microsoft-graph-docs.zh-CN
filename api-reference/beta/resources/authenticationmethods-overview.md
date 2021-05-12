---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 1c0d0476ba7917caf407599d5c4ab8180a8d1795
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335616"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD 身份验证方法 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法是用户在 AD Azure Active Directory (中) 。 Azure AD 中的身份验证方法包括密码和手机（例如，短信和语音呼叫），目前可在 Microsoft Graph 中对这些方法进行管理，此外还有 FIDO2 安全密钥和 Microsoft Authenticator 应用。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 API 用于管理用户的身份验证方法。 例如：

* 你可以向用户添加电话号码。 然后，如果用户按策略短信该电话号码，则用户可以使用该电话号码进行语音呼叫身份验证。
* 可以更新该号码，也可以将其从用户中删除。
* 可以启用或禁用登录短信号码。
* 可以重置用户密码。
* 可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了该密钥，则将其删除。
* 可以检索用户注册Microsoft Authenticator的详细信息，如果用户丢失了电话，可将其删除。
* 你可以向用户添加电子邮件地址。 然后，用户可以在 SSPR Self-Service过程中使用该 (密码) 一部分。
* 你可以更新该电子邮件，也可以从用户中删除它。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| 密码当前是 Azure AD 中默认的主身份验证方法。|重置用户密码|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|用户可以使用电话进行身份验证，短信[策略](/azure/active-directory/authentication/concept-authentication-methods#phone-options) (允许的语音呼叫) 。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用主移动电话短信登录。|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|FIDO2 安全密钥可用于登录 Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator Azure AD 的登录或执行多重身份验证时，用户可以使用密码|删除Microsoft Authenticator身份验证方法。|
|[passwordlessmicrosoftauthenticatorauthentication (](passwordlessmicrosoftauthenticatorauthenticationmethod.md) 弃) |Microsoft Authenticator无电话用户登录 Azure AD 时可以使用无密码登录|删除无密码电话登录身份验证方法。|
|[emailAuthenticationMethod](emailauthenticationmethod.md)|电子邮件地址可以是用户作为 SSPR 密码重置过程Self-Service密码重置 (用户) 过程。|请参阅用户的身份验证电子邮件地址。 向用户添加、更新或删除电子邮件地址。|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|WindowsHello for Business 是一种无密码登录方法，适用于Windows设备。|请参阅用户已启用 hello 企业Windows的设备。 删除Windows Hello 企业凭据。|
|[temporaryaccesspassauthenticationmethod](temporaryaccesspassauthenticationmethod.md)|临时访问传递是一种有时间限制的密码，用作强凭据并允许载入无密码凭据。 | 为用户设置新的临时访问传递。|

Microsoft beta 版中尚不支持以下Graph方法。

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|硬件令牌 | 允许用户使用提供一次代码的物理设备执行多重身份验证。 | 获取分配给用户的硬件令牌。|
|软件令牌 | 允许用户使用满足一系列函数的一次代码的应用程序执行多重身份验证。 | 获取并删除分配给用户的软件令牌。|
|安全问题和解答 | 允许用户在执行自助服务密码重置时验证其身份。 |删除用户注册的安全问题。|
|默认方法 | 表示用户已选择作为执行多重身份验证的默认方法。| 更改用户的默认 MFA 方法。|

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。
