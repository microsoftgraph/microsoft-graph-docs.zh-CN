---
title: 使用身份验证方法使用情况报告 API
description: 身份验证方法使用情况报告可帮助组织了解其最终用户如何使用 Azure Active Directory 功能，如自助密码重置和多重身份验证 (MFA) 。
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: fbf9bc81d37b7f102e46ae47a899403570862660
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523481"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a><span data-ttu-id="d9c6a-103">使用身份验证方法使用情况报告 API</span><span class="sxs-lookup"><span data-stu-id="d9c6a-103">Working with the authentication methods usage report API</span></span>

<span data-ttu-id="d9c6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9c6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9c6a-105">身份验证方法使用情况报告可帮助你了解组织中的用户如何使用 Azure Active Directory (Azure AD) 功能，如自助密码重置和多重身份验证 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-105">The authentication methods usage reports help you understand how users in your organization use Azure Active Directory (Azure AD) capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span>

<span data-ttu-id="d9c6a-106">这些报告提供如下信息：</span><span class="sxs-lookup"><span data-stu-id="d9c6a-106">These reports provide information such as:</span></span>

- <span data-ttu-id="d9c6a-107">您的组织更成功的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-107">Which authentication methods are more successful for your organization.</span></span> 
- <span data-ttu-id="d9c6a-108">最终用户正在运行的错误类型。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-108">What types of errors end users are running into.</span></span>
- <span data-ttu-id="d9c6a-109">您需要运行什么市场活动，以帮助最终用户采用自助密码 rest 和 MFA 的使用。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-109">What campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span>

## <a name="common-requests"></a><span data-ttu-id="d9c6a-110">常见请求</span><span class="sxs-lookup"><span data-stu-id="d9c6a-110">Common requests</span></span>

<span data-ttu-id="d9c6a-111">下表列出了可与此 API 一起使用的一些常见请求。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-111">The following table lists some common requests that you can use with this API.</span></span>

| <span data-ttu-id="d9c6a-112">Operation</span><span class="sxs-lookup"><span data-stu-id="d9c6a-112">Operation</span></span> | <span data-ttu-id="d9c6a-113">在 Graph 浏览器中试用</span><span class="sxs-lookup"><span data-stu-id="d9c6a-113">Try in Graph Explorer</span></span> | <span data-ttu-id="d9c6a-114">说明</span><span class="sxs-lookup"><span data-stu-id="d9c6a-114">Description</span></span> |
| --------- | --- | ----------- |
| [<span data-ttu-id="d9c6a-115">getCredentialUserRegistrationcount</span><span class="sxs-lookup"><span data-stu-id="d9c6a-115">getCredentialUserRegistrationcount</span></span>](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta) | <span data-ttu-id="d9c6a-116">[获取/credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span><span class="sxs-lookup"><span data-stu-id="d9c6a-116">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span></span> | <span data-ttu-id="d9c6a-117">获取注册了自助密码重置和 MFA 的用户数。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-117">Get the number of users registered for self-service password reset and MFA.</span></span> |
| [<span data-ttu-id="d9c6a-118">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="d9c6a-118">getCredentialUsageSummary</span></span>](/graph/api/resources/credentialusagesummary?view=graph-rest-beta) | [<span data-ttu-id="d9c6a-119">获取/credentialusagesummary</span><span class="sxs-lookup"><span data-stu-id="d9c6a-119">GET /credentialusagesummary</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | <span data-ttu-id="d9c6a-120">获取使用自助密码重置的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-120">Get the number of users using self-service password reset.</span></span> |
| [<span data-ttu-id="d9c6a-121">credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="d9c6a-121">credentialUserRegistrationDetails</span></span>](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) | [<span data-ttu-id="d9c6a-122">获取/credentialuserregistrationdetails</span><span class="sxs-lookup"><span data-stu-id="d9c6a-122">GET /credentialuserregistrationdetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | <span data-ttu-id="d9c6a-123">获取自服务密码重置和 MFA 注册活动的用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-123">Get the user details for self-service password reset and MFA registration activities.</span></span> |
| [<span data-ttu-id="d9c6a-124">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="d9c6a-124">userCredentialUsageDetails</span></span>](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) | [<span data-ttu-id="d9c6a-125">获取/usercredentialusagedetails</span><span class="sxs-lookup"><span data-stu-id="d9c6a-125">GET /usercredentialusagedetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | <span data-ttu-id="d9c6a-126">获取所有自助密码重置活动的用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-126">Get user details for all self-service password reset activities.</span></span> |

## <a name="licenses"></a><span data-ttu-id="d9c6a-127">许可证</span><span class="sxs-lookup"><span data-stu-id="d9c6a-127">Licenses</span></span>

<span data-ttu-id="d9c6a-128">使用情况报告可用于在租户中利用自助密码重置和 MFA 的许可功能。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-128">Usage reports are available for licensed features that take advantage of self-service password reset and MFA in your tenant.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d9c6a-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d9c6a-129">Next steps</span></span>

- <span data-ttu-id="d9c6a-130">了解如何 [部署 Azure Active Directory 自助服务密码重置](/azure/active-directory/authentication/howto-sspr-deployment)。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-130">Learn how to [deploy Azure Active Directory self-service password reset](/azure/active-directory/authentication/howto-sspr-deployment).</span></span>
- <span data-ttu-id="d9c6a-131">了解如何部署 [Azure Active DIRECTORY MFA](/azure/active-directory/authentication/howto-mfa-getstarted)。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-131">Learn how to deploy [Azure Active Directory MFA](/azure/active-directory/authentication/howto-mfa-getstarted).</span></span>
- <span data-ttu-id="d9c6a-132">了解如何启用 [组合的安全信息注册](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)。</span><span class="sxs-lookup"><span data-stu-id="d9c6a-132">Learn how to enable [combined security info registration](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span></span>