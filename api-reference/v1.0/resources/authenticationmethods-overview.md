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
# <a name="azure-ad-authentication-methods-api-overview"></a><span data-ttu-id="48590-103">Azure AD 身份验证方法 API 概述</span><span class="sxs-lookup"><span data-stu-id="48590-103">Azure AD authentication methods API overview</span></span>

<span data-ttu-id="48590-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48590-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48590-105">[身份验证](/azure/active-directory/authentication/concept-authentication-methods) 方法是用户在 Azure Active Directory (AD) 。</span><span class="sxs-lookup"><span data-stu-id="48590-105">[Authentication methods](/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (AD).</span></span> <span data-ttu-id="48590-106">Azure AD 中的身份验证方法包括密码和电话 (例如，短信和语音呼叫) ，这些呼叫现在在 Microsoft Graph beta 终结点中可管理，此外，还包括 FIDO2 安全密钥和 Microsoft Authenticator 应用等。</span><span class="sxs-lookup"><span data-stu-id="48590-106">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph beta endpoint today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="48590-107">身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。</span><span class="sxs-lookup"><span data-stu-id="48590-107">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="48590-108">身份验证方法 API 用于管理用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="48590-108">The authentication method APIs are used to manage a user's authentication methods.</span></span> <span data-ttu-id="48590-109">例如：</span><span class="sxs-lookup"><span data-stu-id="48590-109">For example:</span></span>

* <span data-ttu-id="48590-110">可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了该密钥，则将其删除。</span><span class="sxs-lookup"><span data-stu-id="48590-110">You can retrieve details of a user's FIDO2 Security Key, and delete it if the user has lost the key.</span></span>
* <span data-ttu-id="48590-111">可以检索用户的 Microsoft Authenticator 注册的详细信息，如果用户丢失了手机，则将其删除。</span><span class="sxs-lookup"><span data-stu-id="48590-111">You can retrieve details of a user's Microsoft Authenticator registration, and delete it if the user has lost the phone.</span></span>

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="48590-112">可以在 Microsoft Graph 中管理哪些身份验证方法？</span><span class="sxs-lookup"><span data-stu-id="48590-112">What authentication methods can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="48590-113">身份验证方法</span><span class="sxs-lookup"><span data-stu-id="48590-113">Authentication method</span></span>       | <span data-ttu-id="48590-114">说明</span><span class="sxs-lookup"><span data-stu-id="48590-114">Description</span></span> |<span data-ttu-id="48590-115">示例</span><span class="sxs-lookup"><span data-stu-id="48590-115">Examples</span></span>     |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="48590-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="48590-116">fido2AuthenticationMethod</span></span>](fido2authenticationmethod.md)|<span data-ttu-id="48590-117">FIDO2 安全密钥可用于登录 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="48590-117">A FIDO2 Security Key can be used by a user to sign-in to Azure AD.</span></span>|<span data-ttu-id="48590-118">删除丢失的 FIDO2 安全密钥。</span><span class="sxs-lookup"><span data-stu-id="48590-118">Delete a lost FIDO2 Security Key.</span></span>|
|[<span data-ttu-id="48590-119">microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="48590-119">microsoftAuthenticatorAuthenticationMethod</span></span>](microsoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="48590-120">用户可以使用 Microsoft Authenticator 登录或对 Azure AD 执行多重身份验证</span><span class="sxs-lookup"><span data-stu-id="48590-120">Microsoft Authenticator can be used by a user to sign-in or perform multi-factor authentication to Azure AD</span></span>|<span data-ttu-id="48590-121">删除 Microsoft Authenticator 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="48590-121">Delete a Microsoft Authenticator authentication method.</span></span>|
|[<span data-ttu-id="48590-122">windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="48590-122">windowsHelloForBusinessAuthenticationMethod</span></span>](windowsHelloForBusinessAuthenticationMethod.md)|<span data-ttu-id="48590-123">Windows Hello 企业应用在 Windows 设备上是一种无密码登录方法。</span><span class="sxs-lookup"><span data-stu-id="48590-123">Windows Hello for Business is a passwordless sign-in method on Windows devices.</span></span>|<span data-ttu-id="48590-124">请参阅用户已启用 Windows Hello 企业登录的设备。</span><span class="sxs-lookup"><span data-stu-id="48590-124">See devices where a user has enabled Windows Hello for Business sign-in.</span></span> <span data-ttu-id="48590-125">删除 Windows Hello 企业版本凭据。</span><span class="sxs-lookup"><span data-stu-id="48590-125">Delete a Windows Hello for Business credential.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="48590-126">后续步骤</span><span class="sxs-lookup"><span data-stu-id="48590-126">Next steps</span></span>

* <span data-ttu-id="48590-127">查看身份验证方法类型及其各种方法。</span><span class="sxs-lookup"><span data-stu-id="48590-127">Review the authentication method types and their various methods.</span></span>
* <span data-ttu-id="48590-128">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。</span><span class="sxs-lookup"><span data-stu-id="48590-128">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>