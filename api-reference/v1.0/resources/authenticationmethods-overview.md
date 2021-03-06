---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 2c6c69522bf78b6e20a09e6e1d8310565041f333
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335595"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD 身份验证方法 API 概述

命名空间：microsoft.graph

[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法是用户在 AD Azure Active Directory (中) 。 Azure AD 中的身份验证方法包括密码和电话 (例如，短信 和语音呼叫) ，这些呼叫现在在 Microsoft Graph beta 终结点中可管理，此外，还包括 FIDO2 安全密钥和 Microsoft Authenticator 应用等。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 API 用于管理用户的身份验证方法。 例如：

* 可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了该密钥，则将其删除。
* 可以检索用户注册Microsoft Authenticator的详细信息，如果用户丢失了电话，可将其删除。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|FIDO2 安全密钥可用于登录 Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator Azure AD 的登录或执行多重身份验证时，用户可以使用密码|删除Microsoft Authenticator身份验证方法。|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|WindowsHello for Business 是一种无密码登录方法，适用于Windows设备。|请参阅用户已启用 hello 企业Windows的设备。 删除Windows Hello 企业凭据。|

Microsoft Graph v1.0 中尚不支持以下身份验证方法。

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|Password | 密码当前是 Azure AD 中默认的主身份验证方法。|重置用户密码。|
|phoneAuthenticationMethod (尚不支持)  |用户可以使用电话进行身份验证，短信[策略](/azure/active-directory/authentication/concept-authentication-methods#phone-options) (允许的语音呼叫) 。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用主移动电话短信登录。|
|电子邮件 |电子邮件地址可以是用户作为 SSPR 密码重置过程Self-Service密码重置 (用户) 过程。|请参阅用户的身份验证电子邮件地址。 向用户添加、更新或删除电子邮件地址。|
|临时访问传递 |临时访问传递是一种有时间限制的密码，用作强凭据并允许载入无密码凭据。 | 为用户设置新的临时访问传递。|
|硬件令牌 | 允许用户使用提供一次代码的物理设备执行多重身份验证。 | 获取分配给用户的硬件令牌。|
|软件令牌 | 允许用户使用满足一系列函数的一次代码的应用程序执行多重身份验证。 | 获取并删除分配给用户的软件令牌。|
|安全问题和解答 | 允许用户在执行自助服务密码重置时验证其身份。 |删除用户注册的安全问题。|
|默认方法 | 表示用户已选择作为执行多重身份验证的默认方法。| 更改用户的默认 MFA 方法。|

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。
