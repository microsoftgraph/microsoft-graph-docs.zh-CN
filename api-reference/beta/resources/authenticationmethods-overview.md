---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 98de9847ec0e50cb17c6ab64423d891bd3c5e8a3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874303"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD 身份验证方法 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[身份验证方法是](/azure/active-directory/authentication/concept-authentication-methods) 用户在 Azure Active Directory (AD) 。 Azure AD 中的身份验证方法包括密码和手机（例如，短信和语音呼叫），目前可在 Microsoft Graph 中对这些方法进行管理，此外还有 FIDO2 安全密钥和 Microsoft Authenticator 应用。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 API 用于管理用户的身份验证方法。 例如：

* 你可以向用户添加电话号码。 然后，如果用户通过策略启用该电话号码，则他们可以使用该电话号码进行短信和语音呼叫身份验证。
* 可以更新该号码，也可以将其从用户中删除。
* 您可以启用或禁用短信登录号码。
* 可以重置用户密码。
* 可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了该密钥，则将其删除。
* 可以检索用户的 Microsoft Authenticator 注册的详细信息，如果用户丢失了电话，则将其删除。
* 您可以向用户添加电子邮件地址。 然后，用户可以将电子邮件用作 SSPR Self-Service密码重置 (的) 一部分。
* 您可以更新该电子邮件，也可以将其从用户中删除。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>可以在 Microsoft Graph 中管理哪些身份验证方法？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| 密码当前是 Azure AD 中默认的主身份验证方法。|重置用户密码|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|用户可以使用电话使用短信或语音呼叫进行身份验证， ([](/azure/active-directory/authentication/concept-authentication-methods#phone-options)策略策略允许) 。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用短信登录的主移动电话。|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|FIDO2 安全密钥可用于登录 Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|用户可以使用 Microsoft Authenticator 登录或对 Azure AD 执行多重身份验证|删除 Microsoft Authenticator 身份验证方法。|
|[passwordlessmicrosoftauthenticatorauthenticationmethod (](passwordlessmicrosoftauthenticatorauthenticationmethod.md) 已弃) |用户可以使用 Microsoft Authenticator 无密码电话登录登录 Azure AD|删除无密码电话登录身份验证方法。|
|[emailAuthenticationMethod](emailauthenticationmethod.md)|电子邮件地址可以是用户作为 SSPR Self-Service密码重置 (一) 一部分。|查看用户的身份验证电子邮件地址。 向用户添加、更新或删除电子邮件地址。|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello 企业应用是 Windows 设备上一种无密码登录方法。|查看用户已启用 Windows Hello 企业登录的设备。 删除 Windows Hello 企业企业凭据。|

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。