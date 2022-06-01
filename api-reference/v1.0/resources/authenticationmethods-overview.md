---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 6e4cbf0a80eec6e9e74d0d217847e5d4edb458a1
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819760"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD 身份验证方法 API 概述

命名空间：microsoft.graph

[身份验证方法](/azure/active-directory/authentication/concept-authentication-methods)是用户在AZURE ACTIVE DIRECTORY (AD) 中进行身份验证的方式。 Azure AD 中的身份验证方法包括密码和电话 (，例如，短信和语音呼叫) （在 Microsoft Graph beta 终结点中可管理）以及其他许多方法，例如 FIDO2 安全密钥和Microsoft Authenticator应用。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 API 用于管理用户的身份验证方法。 例如：

* 可以检索用户的 FIDO2 安全密钥的详细信息，并在用户丢失密钥时将其删除。
* 可以检索用户Microsoft Authenticator注册的详细信息，并在用户丢失手机时将其删除。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>可在 Microsoft Graph 中管理哪些身份验证方法？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|用户可以使用 FIDO2 安全密钥登录到 Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|用户可以使用Microsoft Authenticator登录或对 Azure AD 执行多重身份验证|删除Microsoft Authenticator身份验证方法。|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello 企业版是Windows设备上的无密码登录方法。|请参阅用户已启用Windows Hello 企业版登录的设备。 删除Windows Hello 企业版凭据。|

Microsoft Graph v1.0 尚不支持以下身份验证方法。

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|Password | 密码目前是 Azure AD 中的默认主身份验证方法。|重置用户的密码。|
|phoneAuthenticationMethod (尚不支持)  |用户可以使用手机使用[策略) 允许的短信或语音呼叫](/azure/active-directory/authentication/concept-authentication-methods#phone-options) (进行身份验证。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用主移动电话以短信登录。|
|电子邮件 |作为Self-Service密码重置 (SSPR) 过程的一部分，用户可以使用电子邮件地址。|请参阅用户的身份验证电子邮件地址。 向用户添加、更新或删除电子邮件地址。|
|临时访问通行证 |临时访问密码是一个时间限制的密码，用作强凭据并允许载入无密码凭据。 | 在用户身上设置新的临时访问权限。|
|硬件令牌 | 允许用户使用提供一次性代码的物理设备执行多重身份验证。 | 获取分配给用户的硬件令牌。|
|软件令牌 | 允许用户使用支持 OAUTH 规范并提供一次性代码的应用程序执行多重身份验证。 | 获取并删除分配给用户的软件令牌。|
|安全问题和答案 | 允许用户在执行自助式密码重置时验证其标识。 |删除用户注册的安全问题。|
|Default 方法 | 表示用户为执行多重身份验证而选择的默认方法。| 更改用户的默认 MFA 方法。 <br/> **注意：** 目前仅通过使用 **StrongAuthenticationMethods** 属性的 MSOL `Get-MsolUser` 和 `Set-MsolUser` cmdlet 来管理默认方法的详细信息。 |
|需要重新注册 MFA | 表示一个配置，该配置要求在用户下次登录时，系统会请求他们设置新的 MFA 身份验证方法。| 允许用户设置新的 MFA 方法，例如，如果他们更改了身份验证设备。 <br/> **注意：** 此功能目前仅通过使用 **StrongAuthenticationMethods** 属性的 MSOL`Set-MsolUser` cmdlet 受支持。 |

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 在[Graph资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。
