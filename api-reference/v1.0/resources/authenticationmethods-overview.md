---
title: Azure AD身份验证方法 API 概述
description: 身份验证方法是用户如何Azure AD。
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 88542ae3571d4c718c0f163d7fd06927fa22501e
ms.sourcegitcommit: 709d2e3069765c2e570ac1128847c165ab233aa8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2022
ms.locfileid: "62184085"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD身份验证方法 API 概述

命名空间：microsoft.graph

[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法是用户在 AD Azure Active Directory (中) 。 Azure AD 中的身份验证方法包括密码和电话 (例如，短信和语音呼叫) ，这些呼叫现在在 Microsoft Graph beta 终结点中可管理，此外，还包括 FIDO2 安全密钥和 Microsoft Authenticator 应用等。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 API 用于管理用户的身份验证方法。 例如：

* 可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了该密钥，则将其删除。
* 可以检索用户注册Microsoft Authenticator的详细信息，如果用户丢失了电话，可将其删除。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|FIDO2 安全密钥可用于登录Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator用户可用于登录或对用户执行多重Azure AD|删除Microsoft Authenticator身份验证方法。|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello For Business 是设备上无密码Windows方法。|请参阅用户已启用适用于Windows Hello登录的设备。 删除Windows Hello企业凭据。|

Microsoft Graph v1.0 中尚不支持以下身份验证方法。

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|Password | 密码当前是默认的主要身份验证方法Azure AD。|重置用户的密码。|
|phoneAuthenticationMethod (尚不支持)  |用户可以使用电话使用短信或语音呼叫进行身份验证， ([](/azure/active-directory/authentication/concept-authentication-methods#phone-options)策略策略允许) 。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用用于短信登录的主移动电话。|
|电子邮件 |电子邮件地址可以是用户作为 SSPR Self-Service密码重置 (的) 一部分。|请参阅用户的身份验证电子邮件地址。 向用户添加、更新或删除电子邮件地址。|
|临时访问传递 |临时访问传递是一种有时间限制的密码，用作强凭据并允许载入无密码凭据。 | 为用户设置新的临时访问传递。|
|硬件令牌 | 允许用户使用提供一次代码的物理设备执行多重身份验证。 | 获取分配给用户的硬件令牌。|
|软件令牌 | 允许用户使用满足一系列函数的一次代码的应用程序执行多重身份验证。 | 获取并删除分配给用户的软件令牌。|
|安全问题和解答 | 允许用户在执行自助服务密码重置时验证其身份。 |删除用户注册的安全问题。|
|默认方法 | 表示用户已选择作为执行多重身份验证的默认方法。| 更改用户的默认 MFA 方法。 <br/> **注意：** 当前仅支持通过 MSOL 和 `Get-MsolUser` `Set-MsolUser` cmdlet（使用 **StrongAuthenticationMethods** 属性）管理默认方法的详细信息。 |
|需要重新注册 MFA | 表示一种配置，要求在用户下次登录时，要求他们设置新的 MFA 身份验证方法。| 允许用户设置新的 MFA 方法，例如，如果他们更改了身份验证设备。 <br/> **注意：** 此功能当前仅支持使用 `Set-MsolUser` **StrongAuthenticationMethods** 属性的 MSOL cmdlet。 |

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 在资源管理器 中Graph [API。](https://developer.microsoft.com/graph/graph-explorer)
