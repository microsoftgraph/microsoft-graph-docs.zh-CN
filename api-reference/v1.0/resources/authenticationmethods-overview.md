---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 6027e03a4c78c5359db77ee9c263c9e98f412a9f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469120"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD 身份验证方法 API 概述

命名空间：microsoft.graph

[身份验证](/azure/active-directory/authentication/concept-authentication-methods) 方法是用户在 Azure Active Directory (AD) 。 Azure AD 中的身份验证方法包括密码和电话 (例如，短信和语音呼叫) ，这些呼叫现在在 Microsoft Graph beta 终结点中可管理，此外，还包括 FIDO2 安全密钥和 Microsoft Authenticator 应用等。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 API 用于管理用户的身份验证方法。 例如：

* 可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了该密钥，则将其删除。
* 可以检索用户的 Microsoft Authenticator 注册的详细信息，如果用户丢失了手机，则将其删除。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>可以在 Microsoft Graph 中管理哪些身份验证方法？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|FIDO2 安全密钥可用于登录 Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|用户可以使用 Microsoft Authenticator 登录或对 Azure AD 执行多重身份验证|删除 Microsoft Authenticator 身份验证方法。|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello 企业应用在 Windows 设备上是一种无密码登录方法。|请参阅用户已启用 Windows Hello 企业登录的设备。 删除 Windows Hello 企业版本凭据。|

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。