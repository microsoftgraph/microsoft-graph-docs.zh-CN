---
title: Azure AD身份验证方法 API 概述
description: 身份验证方法是用户通过身份验证Azure AD。
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 080fa60c83edd0b1c5340102fe4f6886dc1e7e08
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60486640"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD身份验证方法 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法是用户在 AD Azure Active Directory (中) 。 Azure AD 中的身份验证方法包括密码和手机（例如，短信和语音呼叫），目前可在 Microsoft Graph 中对这些方法进行管理，此外还有 FIDO2 安全密钥和 Microsoft Authenticator 应用。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 API 用于管理用户的身份验证方法。 例如：

* 你可以向用户添加电话号码。 然后，如果用户按策略启用其使用，则用户可以使用该电话号码进行短信和语音呼叫身份验证。
* 可以更新该号码，也可以将其从用户中删除。
* 你可以启用或禁用短信登录号码。
* 可以重置用户密码。
* 可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了该密钥，则将其删除。
* 可以检索用户注册Microsoft Authenticator的详细信息，如果用户丢失了电话，则将其删除。
* 你可以向用户添加电子邮件地址。 然后，用户可以将电子邮件用作 SSPR Self-Service密码重置 (的) 一部分。
* 你可以更新该电子邮件，也可以从用户中删除它。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| 密码当前是默认的主要身份验证方法Azure AD。|重置用户密码|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|用户可以使用电话通过短信或语音呼叫进行身份验证， ([](/azure/active-directory/authentication/concept-authentication-methods#phone-options)策略策略允许) 。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用用于短信登录的主移动电话。|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|FIDO2 安全密钥可用于登录Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator用户可以使用密码登录或执行多重身份验证Azure AD|删除Microsoft Authenticator身份验证方法。|
|[passwordlessmicrosoftauthenticatorauthentication (](passwordlessmicrosoftauthenticatorauthenticationmethod.md) 弃) |Microsoft Authenticator无电话用户可以使用无密码登录登录Azure AD|删除无密码电话登录身份验证方法。|
|[emailAuthenticationMethod](emailauthenticationmethod.md)|用户可以将电子邮件地址用作 SSPR Self-Service密码重置 (的) 一部分。|请参阅用户的身份验证电子邮件地址。 向用户添加、更新或删除电子邮件地址。|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello For Business 是设备上无密码Windows方法。|请参阅用户已启用适用于Windows Hello登录的设备。 删除Windows Hello企业凭据。|
|[temporaryaccesspassauthenticationmethod](temporaryaccesspassauthenticationmethod.md)|临时访问传递是一种有时间限制的密码，用作强凭据并允许载入无密码凭据。 | 为用户设置新的临时访问传递。|
|[softwareOathAuthenticationMethod](../resources/softwareoathauthenticationmethod.md)| 允许用户使用支持一次代码且支持一次代码的应用程序执行多重身份验证。 | 获取并删除分配给用户的软件令牌。|

Microsoft beta 版中尚不支持以下Graph方法。

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|硬件令牌 | 允许用户使用提供一次代码的物理设备执行多重身份验证。 | 获取分配给用户的硬件令牌。|
|安全问题和解答 | 允许用户在执行自助服务密码重置时验证其身份。 |删除用户注册的安全问题。|
|默认方法 | 表示用户已选择作为执行多重身份验证的默认方法。| 更改用户的默认 MFA 方法。|

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。
