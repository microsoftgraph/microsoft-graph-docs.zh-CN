---
title: Azure AD 身份验证方法策略 API 概述
description: 身份验证方法策略定义 Azure AD 中的用户可以使用哪些身份验证方法。
localization_priority: Normal
author: mmcla
ms.author: michmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 1446603a027085902d5af27a33727bbec03f4496
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515434"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="a27f1-103">Azure AD 身份验证方法策略 API 概述</span><span class="sxs-lookup"><span data-stu-id="a27f1-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="a27f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a27f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a27f1-105">身份验证方法策略定义[](/azure/active-directory/authentication/concept-authentication-methods)身份验证方法，以及允许用户使用它们登录并执行 Azure Active Directory (Azure AD) 中的多重身份验证 (MFA) 。</span><span class="sxs-lookup"><span data-stu-id="a27f1-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="a27f1-106">可以在 Microsoft Graph 中管理的身份验证方法策略包括 FIDO2 安全密钥和 Microsoft Authenticator 应用的无密码电话登录。</span><span class="sxs-lookup"><span data-stu-id="a27f1-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="a27f1-107">身份验证方法策略 API 用于管理策略设置。</span><span class="sxs-lookup"><span data-stu-id="a27f1-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="a27f1-108">例如：</span><span class="sxs-lookup"><span data-stu-id="a27f1-108">For example:</span></span>

* <span data-ttu-id="a27f1-109">定义可在 Azure AD 租户中使用的 FIDO2 安全密钥的类型。</span><span class="sxs-lookup"><span data-stu-id="a27f1-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="a27f1-110">定义允许使用 FIDO2 安全密钥或无密码电话登录登录 Azure AD 的用户或用户组。</span><span class="sxs-lookup"><span data-stu-id="a27f1-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="a27f1-111">可以在 Microsoft Graph 中管理哪些身份验证方法策略？</span><span class="sxs-lookup"><span data-stu-id="a27f1-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="a27f1-112">身份验证方法策略</span><span class="sxs-lookup"><span data-stu-id="a27f1-112">Authentication method policy</span></span>       | <span data-ttu-id="a27f1-113">说明</span><span class="sxs-lookup"><span data-stu-id="a27f1-113">Description</span></span> |
|:---------------------------|:------------|
|[<span data-ttu-id="a27f1-114">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="a27f1-114">smsAuthenticationMethodConfiguration</span></span>](smsAuthenticationMethodConfiguration.md)| <span data-ttu-id="a27f1-115">定义可以在 Azure AD 租户上使用短信的用户。</span><span class="sxs-lookup"><span data-stu-id="a27f1-115">Define users who can use Text Message on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="a27f1-116">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="a27f1-116">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="a27f1-117">定义 FIDO2 安全密钥限制以及可以使用它们登录 Azure AD 的用户。</span><span class="sxs-lookup"><span data-stu-id="a27f1-117">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="a27f1-118">microsoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="a27f1-118">microsoftauthenticatorauthenticationmethodconfiguration</span></span>](microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="a27f1-119">定义可在 Azure AD 租户上使用 Microsoft Authenticator 的用户。</span><span class="sxs-lookup"><span data-stu-id="a27f1-119">Define users who can use Microsoft Authenticator on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="a27f1-120">emailauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="a27f1-120">emailauthenticationmethodconfiguration</span></span>](emailauthenticationmethodconfiguration.md)|<span data-ttu-id="a27f1-121">定义可在 Azure AD 租户上使用电子邮件 OTP 的用户。</span><span class="sxs-lookup"><span data-stu-id="a27f1-121">Define users who can use email OTP on the Azure AD tenant.</span></span>|
|<span data-ttu-id="a27f1-122">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (弃) </span><span class="sxs-lookup"><span data-stu-id="a27f1-122">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (deprecated)</span></span>|<span data-ttu-id="a27f1-123">定义可以使用无密码电话登录登录 Azure AD 的用户。</span><span class="sxs-lookup"><span data-stu-id="a27f1-123">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="a27f1-124">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="a27f1-124">temporaryaccesspassauthenticationmethodconfiguration</span></span>](temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="a27f1-125">定义可以使用临时访问通道登录 Azure AD 的用户。</span><span class="sxs-lookup"><span data-stu-id="a27f1-125">Define users who can use Temporary Access Pass to sign in to Azure AD.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="a27f1-126">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a27f1-126">Next steps</span></span>

* <span data-ttu-id="a27f1-127">请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="a27f1-127">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
