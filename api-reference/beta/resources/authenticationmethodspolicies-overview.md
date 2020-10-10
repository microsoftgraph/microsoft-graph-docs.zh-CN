---
title: Azure AD 身份验证方法策略 API 概述
description: 身份验证方法策略定义了 Azure AD 中的用户可以使用哪些身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 1a4c5c94999885ba01112f6f18bea96e93a5e77b
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418267"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="7d250-103">Azure AD 身份验证方法策略 API 概述</span><span class="sxs-lookup"><span data-stu-id="7d250-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="7d250-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d250-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d250-105">身份验证方法策略定义 [身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) 以及允许使用它们登录并在 Azure Active Directory (azure AD) 中执行多重身份验证 (MFA) 的用户。</span><span class="sxs-lookup"><span data-stu-id="7d250-105">Authentication methods policies define [authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="7d250-106">可以在 Microsoft Graph 中管理的身份验证方法策略包括 FIDO2 Security Keys and Passwordless Phone 登录与 Microsoft 鉴别应用程序。</span><span class="sxs-lookup"><span data-stu-id="7d250-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="7d250-107">身份验证方法策略 Api 用于管理策略设置。</span><span class="sxs-lookup"><span data-stu-id="7d250-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="7d250-108">例如：</span><span class="sxs-lookup"><span data-stu-id="7d250-108">For example:</span></span>

* <span data-ttu-id="7d250-109">定义可在 Azure AD 租户中使用的 FIDO2 安全密钥的类型。</span><span class="sxs-lookup"><span data-stu-id="7d250-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="7d250-110">定义允许使用 FIDO2 Security Keys 或 Passwordless Phone 登录以登录到 Azure AD 的用户或用户组。</span><span class="sxs-lookup"><span data-stu-id="7d250-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="7d250-111">可以在 Microsoft Graph 中管理哪些身份验证方法策略？</span><span class="sxs-lookup"><span data-stu-id="7d250-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="7d250-112">身份验证方法策略</span><span class="sxs-lookup"><span data-stu-id="7d250-112">Authentication method policy</span></span>       | <span data-ttu-id="7d250-113">说明</span><span class="sxs-lookup"><span data-stu-id="7d250-113">Description</span></span> |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="7d250-114">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="7d250-114">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="7d250-115">定义 FIDO2 安全密钥限制和可使用这些限制登录到 Azure AD 的用户。</span><span class="sxs-lookup"><span data-stu-id="7d250-115">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="7d250-116">passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="7d250-116">passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration</span></span>](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="7d250-117">定义可使用 Passwordless Phone 登录登录 Azure AD 的用户。</span><span class="sxs-lookup"><span data-stu-id="7d250-117">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="7d250-118">后续步骤</span><span class="sxs-lookup"><span data-stu-id="7d250-118">Next steps</span></span>

* <span data-ttu-id="7d250-119">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。</span><span class="sxs-lookup"><span data-stu-id="7d250-119">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
