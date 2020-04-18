---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 73f4bb06d15c6b2e41226e872b71ba417de1076b
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557904"
---
# <a name="azure-ad-authentication-methods-api-overview"></a><span data-ttu-id="46c35-103">Azure AD 身份验证方法 API 概述</span><span class="sxs-lookup"><span data-stu-id="46c35-103">Azure AD authentication methods API overview</span></span>

<span data-ttu-id="46c35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46c35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46c35-105">[身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods)是用户在 Azure Active DIRECTORY （AD）中进行身份验证的方法。</span><span class="sxs-lookup"><span data-stu-id="46c35-105">[Authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (AD).</span></span> <span data-ttu-id="46c35-106">Azure AD 中的身份验证方法包括密码和电话（例如，SMS 和语音呼叫），这些方法可在 Microsoft Graph 中进行管理，如 FIDO2 安全密钥和 Microsoft 身份验证器应用等许多其他内容。</span><span class="sxs-lookup"><span data-stu-id="46c35-106">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="46c35-107">身份验证方法在主要、第二因素和分步身份验证以及自助密码重置（SSPR）过程中也使用。</span><span class="sxs-lookup"><span data-stu-id="46c35-107">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="46c35-108">身份验证方法 Api 用于管理用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="46c35-108">The authentication method APIs are used to manage a user's authentication methods.</span></span> <span data-ttu-id="46c35-109">例如：</span><span class="sxs-lookup"><span data-stu-id="46c35-109">For example:</span></span>

* <span data-ttu-id="46c35-110">您可以向用户添加电话号码。</span><span class="sxs-lookup"><span data-stu-id="46c35-110">You can add a phone number to a user.</span></span> <span data-ttu-id="46c35-111">如果启用此电话号码，则用户可以通过策略将其用于 SMS 和语音呼叫身份验证。</span><span class="sxs-lookup"><span data-stu-id="46c35-111">The user can then use that phone number for SMS and voice call authentication if they're enabled to use it by policy.</span></span> 
* <span data-ttu-id="46c35-112">您可以更新该号码，也可以将其从用户中删除。</span><span class="sxs-lookup"><span data-stu-id="46c35-112">You can update that number, or delete it from the user.</span></span>
* <span data-ttu-id="46c35-113">您可以启用或禁用用于 SMS 登录的号码。</span><span class="sxs-lookup"><span data-stu-id="46c35-113">You can enable or disable the number for SMS sign-in.</span></span>
* <span data-ttu-id="46c35-114">您可以重置用户的密码。</span><span class="sxs-lookup"><span data-stu-id="46c35-114">You can reset a user's password.</span></span>

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="46c35-115">可以在 Microsoft Graph 中管理哪些身份验证方法？</span><span class="sxs-lookup"><span data-stu-id="46c35-115">What authentication methods can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="46c35-116">身份验证方法</span><span class="sxs-lookup"><span data-stu-id="46c35-116">Authentication method</span></span>       | <span data-ttu-id="46c35-117">说明</span><span class="sxs-lookup"><span data-stu-id="46c35-117">Description</span></span> |<span data-ttu-id="46c35-118">示例</span><span class="sxs-lookup"><span data-stu-id="46c35-118">Examples</span></span>     |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="46c35-119">passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="46c35-119">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md)| <span data-ttu-id="46c35-120">密码当前是 Azure AD 中默认的主要身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="46c35-120">A password is currently the default primary authentication method in Azure AD.</span></span>|<span data-ttu-id="46c35-121">重置用户密码</span><span class="sxs-lookup"><span data-stu-id="46c35-121">Reset a user's password</span></span>|
|[<span data-ttu-id="46c35-122">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="46c35-122">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md)|<span data-ttu-id="46c35-123">用户可使用电话使用[短信或语音呼叫](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options)进行身份验证（如策略允许）。</span><span class="sxs-lookup"><span data-stu-id="46c35-123">A phone can be used by a user to authenticate using [SMS or voice calls](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (as allowed by policy).</span></span>|<span data-ttu-id="46c35-124">查看用户的身份验证电话号码。</span><span class="sxs-lookup"><span data-stu-id="46c35-124">See a user's authentication phone numbers.</span></span> <span data-ttu-id="46c35-125">向用户添加、更新或删除电话号码。</span><span class="sxs-lookup"><span data-stu-id="46c35-125">Add, update, or remove a phone number to a user.</span></span> <span data-ttu-id="46c35-126">启用或禁用 SMS 登录的主移动电话。</span><span class="sxs-lookup"><span data-stu-id="46c35-126">Enable or disable a primary mobile phone for SMS sign-in.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="46c35-127">后续步骤</span><span class="sxs-lookup"><span data-stu-id="46c35-127">Next steps</span></span>

* <span data-ttu-id="46c35-128">查看身份验证方法类型及其各种方法。</span><span class="sxs-lookup"><span data-stu-id="46c35-128">Review the authentication method types and their various methods.</span></span>
* <span data-ttu-id="46c35-129">请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="46c35-129">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
