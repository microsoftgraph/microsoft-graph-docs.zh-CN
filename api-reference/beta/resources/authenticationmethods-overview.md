---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: bb1dd599143447b597c4f57c93b20f3261ecf303
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034117"
---
# <a name="azure-ad-authentication-methods-api-overview"></a><span data-ttu-id="8f7e2-103">Azure AD 身份验证方法 API 概述</span><span class="sxs-lookup"><span data-stu-id="8f7e2-103">Azure AD authentication methods API overview</span></span>

<span data-ttu-id="8f7e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f7e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f7e2-105">[身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) 是用户在 Azure Active DIRECTORY (AD) 中进行身份验证的方法。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-105">[Authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (AD).</span></span> <span data-ttu-id="8f7e2-106">Azure AD 中的身份验证方法包括密码和手机（例如，短信和语音呼叫），目前可在 Microsoft Graph 中对这些方法进行管理，此外还有 FIDO2 安全密钥和 Microsoft Authenticator 应用。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-106">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="8f7e2-107">身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-107">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="8f7e2-108">身份验证方法 Api 用于管理用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-108">The authentication method APIs are used to manage a user's authentication methods.</span></span> <span data-ttu-id="8f7e2-109">例如：</span><span class="sxs-lookup"><span data-stu-id="8f7e2-109">For example:</span></span>

* <span data-ttu-id="8f7e2-110">您可以向用户添加电话号码。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-110">You can add a phone number to a user.</span></span> <span data-ttu-id="8f7e2-111">如果启用此电话号码，则用户可以通过策略将其用于 SMS 和语音呼叫身份验证。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-111">The user can then use that phone number for SMS and voice call authentication if they're enabled to use it by policy.</span></span> 
* <span data-ttu-id="8f7e2-112">您可以更新该号码，也可以将其从用户中删除。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-112">You can update that number, or delete it from the user.</span></span>
* <span data-ttu-id="8f7e2-113">您可以启用或禁用用于 SMS 登录的号码。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-113">You can enable or disable the number for SMS sign-in.</span></span>
* <span data-ttu-id="8f7e2-114">您可以重置用户的密码。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-114">You can reset a user's password.</span></span>

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="8f7e2-115">可以在 Microsoft Graph 中管理哪些身份验证方法？</span><span class="sxs-lookup"><span data-stu-id="8f7e2-115">What authentication methods can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="8f7e2-116">身份验证方法</span><span class="sxs-lookup"><span data-stu-id="8f7e2-116">Authentication method</span></span>       | <span data-ttu-id="8f7e2-117">说明</span><span class="sxs-lookup"><span data-stu-id="8f7e2-117">Description</span></span> |<span data-ttu-id="8f7e2-118">示例</span><span class="sxs-lookup"><span data-stu-id="8f7e2-118">Examples</span></span>     |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="8f7e2-119">passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8f7e2-119">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md)| <span data-ttu-id="8f7e2-120">密码当前是 Azure AD 中默认的主要身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-120">A password is currently the default primary authentication method in Azure AD.</span></span>|<span data-ttu-id="8f7e2-121">重置用户密码</span><span class="sxs-lookup"><span data-stu-id="8f7e2-121">Reset a user's password</span></span>|
|[<span data-ttu-id="8f7e2-122">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8f7e2-122">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md)|<span data-ttu-id="8f7e2-123">用户可以使用电话以使用 [SMS 或语音呼叫](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) 进行身份验证， (按策略) 允许。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-123">A phone can be used by a user to authenticate using [SMS or voice calls](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (as allowed by policy).</span></span>|<span data-ttu-id="8f7e2-124">查看用户的身份验证电话号码。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-124">See a user's authentication phone numbers.</span></span> <span data-ttu-id="8f7e2-125">向用户添加、更新或删除电话号码。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-125">Add, update, or remove a phone number to a user.</span></span> <span data-ttu-id="8f7e2-126">启用或禁用 SMS 登录的主移动电话。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-126">Enable or disable a primary mobile phone for SMS sign-in.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="8f7e2-127">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8f7e2-127">Next steps</span></span>

* <span data-ttu-id="8f7e2-128">查看身份验证方法类型及其各种方法。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-128">Review the authentication method types and their various methods.</span></span>
* <span data-ttu-id="8f7e2-129">在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。</span><span class="sxs-lookup"><span data-stu-id="8f7e2-129">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


