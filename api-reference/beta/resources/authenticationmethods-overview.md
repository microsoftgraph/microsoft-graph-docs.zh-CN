---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: a9ef7e2e3ae69cddaf9c5812c5f45ea8f5159f57
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921541"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD 身份验证方法 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[身份验证方法](/azure/active-directory/authentication/concept-authentication-methods) 是用户在 Azure Active DIRECTORY (AD) 中进行身份验证的方法。 Azure AD 中的身份验证方法包括密码和手机（例如，短信和语音呼叫），目前可在 Microsoft Graph 中对这些方法进行管理，此外还有 FIDO2 安全密钥和 Microsoft Authenticator 应用。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 Api 用于管理用户的身份验证方法。 例如：

* 您可以向用户添加电话号码。 如果启用此电话号码，则用户可以通过策略将其用于 SMS 和语音呼叫身份验证。
* 您可以更新该号码，也可以将其从用户中删除。
* 您可以启用或禁用用于 SMS 登录的号码。
* 您可以重置用户的密码。
* 您可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了密钥，则将其删除。
* 您可以检索用户的 Microsoft 身份验证 Passwordless 手机登录注册的详细信息，并在用户丢失电话时删除它。
* 您可以向用户添加电子邮件地址。 然后，用户可以将该电子邮件用作 Self-Service 密码重置 (SSPR) 进程的一部分。
* 您可以更新该电子邮件，或将其从用户中删除。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>可以在 Microsoft Graph 中管理哪些身份验证方法？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| 密码当前是 Azure AD 中默认的主要身份验证方法。|重置用户密码|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|用户可以使用电话以使用 [SMS 或语音呼叫](/azure/active-directory/authentication/concept-authentication-methods#phone-options) 进行身份验证， (按策略) 允许。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用 SMS 登录的主移动电话。|
|[fido2authenticationmethod](fido2authenticationmethod.md)|用户可使用 FIDO2 安全密钥登录 Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[passwordlessmicrosoftauthenticatorauthenticationmethod](passwordlessmicrosoftauthenticatorauthenticationmethod.md)|用户可使用 Microsoft 身份验证 Passwordless 电话登录来登录 Azure AD|删除 Passwordless 电话登录身份验证方法。|
|[emailauthenticationmethod](emailauthenticationmethod.md)|电子邮件地址可以由用户作为 Self-Service 密码重置 (SSPR) 过程的一部分。|查看用户的身份验证电子邮件地址。 向用户添加、更新或删除电子邮件地址。|

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。