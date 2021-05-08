---
title: 使用身份验证方法使用情况报告 API
description: 身份验证方法使用情况报告可帮助组织了解其最终用户如何使用 Azure Active Directory 功能，如自助服务密码重置和 MFA (多重) 。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 53ec8c6046c9682c0bdea607a942cb673671d0b3
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231642"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a><span data-ttu-id="d5afc-103">使用身份验证方法使用情况报告 API</span><span class="sxs-lookup"><span data-stu-id="d5afc-103">Working with the authentication methods usage report API</span></span>

<span data-ttu-id="d5afc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5afc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5afc-105">身份验证方法使用情况报告可帮助你了解贵组织的用户如何使用 Azure Active Directory (Azure AD) 功能，如多重身份验证 (MFA) 、Self-Service 密码重置 (SSPR) 和无密码身份验证。</span><span class="sxs-lookup"><span data-stu-id="d5afc-105">The authentication methods usage reports help you understand how users in your organization use Azure Active Directory (Azure AD) features such as Multi-Factor Authentication (MFA), Self-Service Password Reset (SSPR), and Passwordless authentication.</span></span>

<span data-ttu-id="d5afc-106">这些报告提供以下信息：</span><span class="sxs-lookup"><span data-stu-id="d5afc-106">These reports provide information such as:</span></span>

- <span data-ttu-id="d5afc-107">每个身份验证方法注册的用户数</span><span class="sxs-lookup"><span data-stu-id="d5afc-107">How many users are registered for each authentication method</span></span>
- <span data-ttu-id="d5afc-108">注册多重身份验证、MFA (、SSPR) Self-Service 密码重置 (SSPR) 等功能的用户数。</span><span class="sxs-lookup"><span data-stu-id="d5afc-108">How many users are registered for features such as Multi-Factor Authentication (MFA), Self-Service Password Reset (SSPR), and Passwordless authentication.</span></span>
- <span data-ttu-id="d5afc-109">每个身份验证方法的失败率</span><span class="sxs-lookup"><span data-stu-id="d5afc-109">The failure rates of each authentication method</span></span> 

## <a name="permissions"></a><span data-ttu-id="d5afc-110">权限</span><span class="sxs-lookup"><span data-stu-id="d5afc-110">Permissions</span></span>
<span data-ttu-id="d5afc-111">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="d5afc-111">The following permissions are required to call this API.</span></span> <span data-ttu-id="d5afc-112">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5afc-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5afc-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5afc-113">Permission type</span></span>|<span data-ttu-id="d5afc-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5afc-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5afc-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5afc-115">Delegated (work or school account)</span></span>|<span data-ttu-id="d5afc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5afc-116">Reports.Read.All</span></span><br><span data-ttu-id="d5afc-117">AuditLogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5afc-117">AuditLogs.Read.All</span></span>|
|<span data-ttu-id="d5afc-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5afc-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5afc-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5afc-119">Not supported.</span></span>|
|<span data-ttu-id="d5afc-120">应用</span><span class="sxs-lookup"><span data-stu-id="d5afc-120">Application</span></span>|<span data-ttu-id="d5afc-121">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5afc-121">Reports.Read.All</span></span><br><span data-ttu-id="d5afc-122">AuditLogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5afc-122">AuditLogs.Read.All</span></span>|

<span data-ttu-id="d5afc-123">若要访问 API， [需要以下角色之](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) 一：</span><span class="sxs-lookup"><span data-stu-id="d5afc-123">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="d5afc-124">报表阅读人员</span><span class="sxs-lookup"><span data-stu-id="d5afc-124">Reports reader</span></span>
* <span data-ttu-id="d5afc-125">安全读者</span><span class="sxs-lookup"><span data-stu-id="d5afc-125">Security reader</span></span>
* <span data-ttu-id="d5afc-126">安全管理员</span><span class="sxs-lookup"><span data-stu-id="d5afc-126">Security admin</span></span>
* <span data-ttu-id="d5afc-127">全局读取者</span><span class="sxs-lookup"><span data-stu-id="d5afc-127">Global reader</span></span>
* <span data-ttu-id="d5afc-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d5afc-128">Global admin</span></span>

## <a name="licenses"></a><span data-ttu-id="d5afc-129">许可证</span><span class="sxs-lookup"><span data-stu-id="d5afc-129">Licenses</span></span>

<span data-ttu-id="d5afc-130">需要 Azure AD 高级版 P1 或 P2 许可证才能访问使用情况和见解。</span><span class="sxs-lookup"><span data-stu-id="d5afc-130">An Azure AD Premium P1 or P2 license is required to access usage and insights.</span></span> <span data-ttu-id="d5afc-131">Azure AD Multi-Factor Authentication and self-service password reset (SSPR) licensing information can be found on the [Azure Active Directory pricing site](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="d5afc-131">Azure AD Multi-Factor Authentication and self-service password reset (SSPR) licensing information can be found on the [Azure Active Directory pricing site](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="common-requests"></a><span data-ttu-id="d5afc-132">常见请求</span><span class="sxs-lookup"><span data-stu-id="d5afc-132">Common requests</span></span>

<span data-ttu-id="d5afc-133">下表列出了可用于此 API 的一些常见请求。</span><span class="sxs-lookup"><span data-stu-id="d5afc-133">The following table lists some common requests that you can use with this API.</span></span>

| <span data-ttu-id="d5afc-134">Operation</span><span class="sxs-lookup"><span data-stu-id="d5afc-134">Operation</span></span> | <span data-ttu-id="d5afc-135">在 Graph 浏览器中试用</span><span class="sxs-lookup"><span data-stu-id="d5afc-135">Try in Graph Explorer</span></span> | <span data-ttu-id="d5afc-136">说明</span><span class="sxs-lookup"><span data-stu-id="d5afc-136">Description</span></span> |
| --------- | --- | ----------- |
| [<span data-ttu-id="d5afc-137">getCredentialUserRegistrationcount</span><span class="sxs-lookup"><span data-stu-id="d5afc-137">getCredentialUserRegistrationcount</span></span>](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta&preserve-view=true) | <span data-ttu-id="d5afc-138">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span><span class="sxs-lookup"><span data-stu-id="d5afc-138">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span></span> | <span data-ttu-id="d5afc-139">获取注册自助服务密码重置和 MFA 的用户数。</span><span class="sxs-lookup"><span data-stu-id="d5afc-139">Get the number of users registered for self-service password reset and MFA.</span></span> |
| [<span data-ttu-id="d5afc-140">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="d5afc-140">getCredentialUsageSummary</span></span>](/graph/api/resources/credentialusagesummary?view=graph-rest-beta&preserve-view=true) | [<span data-ttu-id="d5afc-141">GET /credentialusagesummary</span><span class="sxs-lookup"><span data-stu-id="d5afc-141">GET /credentialusagesummary</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | <span data-ttu-id="d5afc-142">获取使用自助服务密码重置的用户数。</span><span class="sxs-lookup"><span data-stu-id="d5afc-142">Get the number of users using self-service password reset.</span></span> |
| [<span data-ttu-id="d5afc-143">credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="d5afc-143">credentialUserRegistrationDetails</span></span>](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta&preserve-view=true) | [<span data-ttu-id="d5afc-144">GET /credentialuserregistrationdetails</span><span class="sxs-lookup"><span data-stu-id="d5afc-144">GET /credentialuserregistrationdetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | <span data-ttu-id="d5afc-145">获取自助服务密码重置和 MFA 注册活动的用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="d5afc-145">Get the user details for self-service password reset and MFA registration activities.</span></span> |
| [<span data-ttu-id="d5afc-146">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="d5afc-146">userCredentialUsageDetails</span></span>](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta&preserve-view=true) | [<span data-ttu-id="d5afc-147">GET /usercredentialusagedetails</span><span class="sxs-lookup"><span data-stu-id="d5afc-147">GET /usercredentialusagedetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | <span data-ttu-id="d5afc-148">获取所有自助服务密码重置活动的用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="d5afc-148">Get user details for all self-service password reset activities.</span></span> |
| [<span data-ttu-id="d5afc-149">usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="d5afc-149">usersRegisteredByFeature</span></span>](/graph/api/resources/userregistrationfeaturesummary?view=graph-rest-beta&preserve-view=true) | <span data-ttu-id="d5afc-150">[GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta)</span><span class="sxs-lookup"><span data-stu-id="d5afc-150">[GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta)</span></span> | <span data-ttu-id="d5afc-151">获取能够进行多重身份验证、自助服务密码重置和无密码身份验证的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d5afc-151">Get the number of users capable of multi-factor authentication, self-service password reset and passwordless authentication.</span></span> |
| [<span data-ttu-id="d5afc-152">usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="d5afc-152">usersRegisteredByMethod</span></span>](/graph/api/resources/userregistrationmethodsummary?view=graph-rest-beta&preserve-view=true) | <span data-ttu-id="d5afc-153">[GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta)</span><span class="sxs-lookup"><span data-stu-id="d5afc-153">[GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta)</span></span> | <span data-ttu-id="d5afc-154">获取针对每个身份验证方法注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="d5afc-154">Get the number of users registered for each authentication method.</span></span> |

## <a name="next-steps"></a><span data-ttu-id="d5afc-155">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d5afc-155">Next steps</span></span>

- <span data-ttu-id="d5afc-156">了解如何部署[Azure Active Directory密码重置。](/azure/active-directory/authentication/howto-sspr-deployment)</span><span class="sxs-lookup"><span data-stu-id="d5afc-156">Learn how to [deploy Azure Active Directory self-service password reset](/azure/active-directory/authentication/howto-sspr-deployment).</span></span>
- <span data-ttu-id="d5afc-157">了解如何部署Azure Active Directory [MFA。](/azure/active-directory/authentication/howto-mfa-getstarted)</span><span class="sxs-lookup"><span data-stu-id="d5afc-157">Learn how to deploy [Azure Active Directory MFA](/azure/active-directory/authentication/howto-mfa-getstarted).</span></span>
- <span data-ttu-id="d5afc-158">了解如何启用组合 [安全信息注册](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)。</span><span class="sxs-lookup"><span data-stu-id="d5afc-158">Learn how to enable [combined security info registration](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span></span>
