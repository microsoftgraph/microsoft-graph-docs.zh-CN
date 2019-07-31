---
title: 使用身份验证方法使用情况报告 API
description: 身份验证方法使用报告可帮助组织了解其最终用户使用的是自服务密码重置和多重身份验证 (MFA) 等 Azure Active Directory 功能的方式。
author: davidmu1
localization_priority: Normal
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 4f8886333d5067abc42a583084726c58ec67a659
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013197"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a><span data-ttu-id="db834-103">使用身份验证方法使用情况报告 API</span><span class="sxs-lookup"><span data-stu-id="db834-103">Working with the authentication methods usage report API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db834-104">身份验证方法使用情况报告可帮助您了解组织中的用户如何使用 Azure Active Directory (Azure AD) 功能, 如自助密码 rest 和多重身份验证 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="db834-104">The authentication methods usage reports help you understand how users in your organization use Azure Active Directory (Azure AD) capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span>

<span data-ttu-id="db834-105">这些报告提供如下信息:</span><span class="sxs-lookup"><span data-stu-id="db834-105">These reports provide information such as:</span></span>

- <span data-ttu-id="db834-106">您的组织更成功的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="db834-106">Which authentication methods are more successful for your organization.</span></span> 
- <span data-ttu-id="db834-107">最终用户正在运行的错误类型。</span><span class="sxs-lookup"><span data-stu-id="db834-107">What types of errors end users are running into.</span></span>
- <span data-ttu-id="db834-108">您需要运行什么市场活动, 以帮助最终用户采用自助密码 rest 和 MFA 的使用。</span><span class="sxs-lookup"><span data-stu-id="db834-108">What campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span>

## <a name="common-requests"></a><span data-ttu-id="db834-109">常见请求</span><span class="sxs-lookup"><span data-stu-id="db834-109">Common requests</span></span>

<span data-ttu-id="db834-110">下表列出了可与此 API 一起使用的一些常见请求。</span><span class="sxs-lookup"><span data-stu-id="db834-110">The following table lists some common requests that you can use with this API.</span></span>

| <span data-ttu-id="db834-111">Operation</span><span class="sxs-lookup"><span data-stu-id="db834-111">Operation</span></span> | <span data-ttu-id="db834-112">在 Graph 浏览器中试用</span><span class="sxs-lookup"><span data-stu-id="db834-112">Try in Graph Explorer</span></span> | <span data-ttu-id="db834-113">说明</span><span class="sxs-lookup"><span data-stu-id="db834-113">Description</span></span> |
| --------- | --- | ----------- |
| [<span data-ttu-id="db834-114">getCredentialUserRegistrationcount</span><span class="sxs-lookup"><span data-stu-id="db834-114">getCredentialUserRegistrationcount</span></span>](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta) | <span data-ttu-id="db834-115">[获取/credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span><span class="sxs-lookup"><span data-stu-id="db834-115">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span></span> | <span data-ttu-id="db834-116">获取注册了自助密码重置和 MFA 的用户数。</span><span class="sxs-lookup"><span data-stu-id="db834-116">Get the number of users registered for self-service password reset and MFA.</span></span> |
| [<span data-ttu-id="db834-117">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="db834-117">getCredentialUsageSummary</span></span>](/graph/api/resources/credentialusagesummary?view=graph-rest-beta) | [<span data-ttu-id="db834-118">获取/credentialusagesummary</span><span class="sxs-lookup"><span data-stu-id="db834-118">GET /credentialusagesummary</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | <span data-ttu-id="db834-119">获取使用自助密码重置的用户数量。</span><span class="sxs-lookup"><span data-stu-id="db834-119">Get the number of users using self-service password reset.</span></span> |
| [<span data-ttu-id="db834-120">credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="db834-120">credentialUserRegistrationDetails</span></span>](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) | [<span data-ttu-id="db834-121">获取/credentialuserregistrationdetails</span><span class="sxs-lookup"><span data-stu-id="db834-121">GET /credentialuserregistrationdetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | <span data-ttu-id="db834-122">获取自服务密码重置和 MFA 注册活动的用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="db834-122">Get the user details for self-service password reset and MFA registration activities.</span></span> |
| [<span data-ttu-id="db834-123">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="db834-123">userCredentialUsageDetails</span></span>](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) | [<span data-ttu-id="db834-124">获取/usercredentialusagedetails</span><span class="sxs-lookup"><span data-stu-id="db834-124">GET /usercredentialusagedetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | <span data-ttu-id="db834-125">获取所有自助密码重置活动的用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="db834-125">Get user details for all self-service password reset activities.</span></span> |

## <a name="licenses"></a><span data-ttu-id="db834-126">许可证</span><span class="sxs-lookup"><span data-stu-id="db834-126">Licenses</span></span>

<span data-ttu-id="db834-127">使用情况报告可用于在租户中利用自助密码重置和 MFA 的许可功能。</span><span class="sxs-lookup"><span data-stu-id="db834-127">Usage reports are available for licensed features that take advantage of self-service password reset and MFA in your tenant.</span></span>

## <a name="next-steps"></a><span data-ttu-id="db834-128">后续步骤</span><span class="sxs-lookup"><span data-stu-id="db834-128">Next steps</span></span>

- <span data-ttu-id="db834-129">了解如何[部署 Azure Active Directory 自助服务密码重置](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment)。</span><span class="sxs-lookup"><span data-stu-id="db834-129">Learn how to [deploy Azure Active Directory self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).</span></span>
- <span data-ttu-id="db834-130">了解如何部署[Azure Active DIRECTORY MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)。</span><span class="sxs-lookup"><span data-stu-id="db834-130">Learn how to deploy [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).</span></span>
- <span data-ttu-id="db834-131">了解如何启用[组合的安全信息注册](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)。</span><span class="sxs-lookup"><span data-stu-id="db834-131">Learn how to enable [combined security info registration](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span></span>



