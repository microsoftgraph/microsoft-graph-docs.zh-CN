---
title: Azure AD 身份验证方法策略 API 概述
description: 身份验证方法策略定义 Azure AD 中的用户可以使用哪些身份验证方法。
localization_priority: Normal
author: mmcla
ms.author: michmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 593cbea196edcbe1c868a337b1dcfa8a1de2afc9
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271825"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="ae144-103">Azure AD 身份验证方法策略 API 概述</span><span class="sxs-lookup"><span data-stu-id="ae144-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="ae144-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae144-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae144-105">身份验证方法策略定义[](/azure/active-directory/authentication/concept-authentication-methods)身份验证方法，以及允许用户使用它们登录并执行 Azure Active Directory (Azure AD) 中的多重身份验证 (MFA) 。</span><span class="sxs-lookup"><span data-stu-id="ae144-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="ae144-106">可以在 Microsoft Graph 中管理的身份验证方法策略包括 FIDO2 安全密钥和 Microsoft Authenticator 应用的无密码电话登录。</span><span class="sxs-lookup"><span data-stu-id="ae144-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="ae144-107">身份验证方法策略 API 用于管理策略设置。</span><span class="sxs-lookup"><span data-stu-id="ae144-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="ae144-108">例如：</span><span class="sxs-lookup"><span data-stu-id="ae144-108">For example:</span></span>

* <span data-ttu-id="ae144-109">定义可在 Azure AD 租户中使用的 FIDO2 安全密钥的类型。</span><span class="sxs-lookup"><span data-stu-id="ae144-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="ae144-110">定义允许使用 FIDO2 安全密钥或无密码电话登录登录 Azure AD 的用户或用户组。</span><span class="sxs-lookup"><span data-stu-id="ae144-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="ae144-111">可以在 Microsoft Graph 中管理哪些身份验证方法策略？</span><span class="sxs-lookup"><span data-stu-id="ae144-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="ae144-112">身份验证方法策略</span><span class="sxs-lookup"><span data-stu-id="ae144-112">Authentication method policy</span></span>       | <span data-ttu-id="ae144-113">说明</span><span class="sxs-lookup"><span data-stu-id="ae144-113">Description</span></span> |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="ae144-114">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae144-114">smsAuthenticationMethodConfiguration</span></span>](smsAuthenticationMethodConfiguration.md)| <span data-ttu-id="ae144-115">定义可以在 Azure AD 租户上使用短信的用户。</span><span class="sxs-lookup"><span data-stu-id="ae144-115">Define users who can use Text Message on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="ae144-116">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="ae144-116">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="ae144-117">定义 FIDO2 安全密钥限制以及可以使用它们登录 Azure AD 的用户。</span><span class="sxs-lookup"><span data-stu-id="ae144-117">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="ae144-118">microsoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="ae144-118">microsoftauthenticatorauthenticationmethodconfiguration</span></span>](microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="ae144-119">定义可在 Azure AD 租户上使用 Microsoft Authenticator 的用户。</span><span class="sxs-lookup"><span data-stu-id="ae144-119">Define users who can use Microsoft Authenticator on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="ae144-120">emailauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="ae144-120">emailauthenticationmethodconfiguration</span></span>](emailauthenticationmethodconfiguration.md)|<span data-ttu-id="ae144-121">定义可在 Azure AD 租户上使用电子邮件 OTP 的用户。</span><span class="sxs-lookup"><span data-stu-id="ae144-121">Define users who can use email OTP on the Azure AD tenant.</span></span>|
|<span data-ttu-id="ae144-122">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (已弃) </span><span class="sxs-lookup"><span data-stu-id="ae144-122">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (deprecated)</span></span>|<span data-ttu-id="ae144-123">定义可以使用无密码电话登录登录 Azure AD 的用户。</span><span class="sxs-lookup"><span data-stu-id="ae144-123">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="ae144-124">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="ae144-124">temporaryaccesspassauthenticationmethodconfiguration</span></span>](temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="ae144-125">定义可以使用临时访问通道登录 Azure AD 的用户。</span><span class="sxs-lookup"><span data-stu-id="ae144-125">Define users who can use Temporary Access Pass to sign in to Azure AD.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="ae144-126">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ae144-126">Next steps</span></span>

* <span data-ttu-id="ae144-127">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。</span><span class="sxs-lookup"><span data-stu-id="ae144-127">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
