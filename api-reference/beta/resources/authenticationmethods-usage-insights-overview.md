---
title: 使用身份验证方法使用情况报告 API
description: 身份验证方法使用情况报告可帮助组织了解其最终用户如何使用 Azure Active Directory 功能，如自助服务密码重置和 MFA (多重) 。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 54f3b823fc1d1c62df07ac6dd9e61f5ea32a2871
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135483"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a><span data-ttu-id="0d909-103">使用身份验证方法使用情况报告 API</span><span class="sxs-lookup"><span data-stu-id="0d909-103">Working with the authentication methods usage report API</span></span>

<span data-ttu-id="0d909-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d909-105">身份验证方法使用情况报告可帮助你了解组织中用户如何使用 Azure Active Directory (Azure AD) 功能，如多重身份验证 (MFA) 、Self-Service 密码重置 (SSPR) 和无密码身份验证。</span><span class="sxs-lookup"><span data-stu-id="0d909-105">The authentication methods usage reports help you understand how users in your organization use Azure Active Directory (Azure AD) features such as Multi-Factor Authentication (MFA), Self-Service Password Reset (SSPR), and Passwordless authentication.</span></span>

<span data-ttu-id="0d909-106">这些报告提供如下信息：</span><span class="sxs-lookup"><span data-stu-id="0d909-106">These reports provide information such as:</span></span>

- <span data-ttu-id="0d909-107">每个身份验证方法注册的用户数</span><span class="sxs-lookup"><span data-stu-id="0d909-107">How many users are registered for each authentication method</span></span>
- <span data-ttu-id="0d909-108">注册多重身份验证 (MFA) 、Self-Service 密码重置 (SSPR) 和无密码身份验证等功能的用户数。</span><span class="sxs-lookup"><span data-stu-id="0d909-108">How many users are registered for features such as Multi-Factor Authentication (MFA), Self-Service Password Reset (SSPR), and Passwordless authentication.</span></span>
- <span data-ttu-id="0d909-109">每个身份验证方法的失败率</span><span class="sxs-lookup"><span data-stu-id="0d909-109">The failure rates of each authentication method</span></span> 

## <a name="permissions"></a><span data-ttu-id="0d909-110">权限</span><span class="sxs-lookup"><span data-stu-id="0d909-110">Permissions</span></span>
<span data-ttu-id="0d909-111">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="0d909-111">The following permissions are required to call this API.</span></span> <span data-ttu-id="0d909-112">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d909-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d909-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d909-113">Permission type</span></span>|<span data-ttu-id="0d909-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d909-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d909-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d909-115">Delegated (work or school account)</span></span>|<span data-ttu-id="0d909-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d909-116">Reports.Read.All</span></span>|
|<span data-ttu-id="0d909-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d909-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d909-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d909-118">Not supported.</span></span>|
|<span data-ttu-id="0d909-119">Application</span><span class="sxs-lookup"><span data-stu-id="0d909-119">Application</span></span>|<span data-ttu-id="0d909-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d909-120">Not supported.</span></span>|

<span data-ttu-id="0d909-121">若要访问 API， [需要以下角色之](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) 一：</span><span class="sxs-lookup"><span data-stu-id="0d909-121">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="0d909-122">报表阅读人员</span><span class="sxs-lookup"><span data-stu-id="0d909-122">Reports reader</span></span>
* <span data-ttu-id="0d909-123">安全读者</span><span class="sxs-lookup"><span data-stu-id="0d909-123">Security reader</span></span>
* <span data-ttu-id="0d909-124">安全管理员</span><span class="sxs-lookup"><span data-stu-id="0d909-124">Security admin</span></span>
* <span data-ttu-id="0d909-125">全局读取者</span><span class="sxs-lookup"><span data-stu-id="0d909-125">Global reader</span></span>
* <span data-ttu-id="0d909-126">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0d909-126">Global admin</span></span>

## <a name="licenses"></a><span data-ttu-id="0d909-127">许可证</span><span class="sxs-lookup"><span data-stu-id="0d909-127">Licenses</span></span>

<span data-ttu-id="0d909-128">需要 Azure AD Premium P1 或 P2 许可证才能访问使用情况和见解。</span><span class="sxs-lookup"><span data-stu-id="0d909-128">An Azure AD Premium P1 or P2 license is required to access usage and insights.</span></span> <span data-ttu-id="0d909-129">Azure AD 多重身份验证和自助服务密码重置 (SSPR) 可在 Azure Active Directory 定价网站上找到 [许可信息](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="0d909-129">Azure AD Multi-Factor Authentication and self-service password reset (SSPR) licensing information can be found on the [Azure Active Directory pricing site](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="common-requests"></a><span data-ttu-id="0d909-130">常见请求</span><span class="sxs-lookup"><span data-stu-id="0d909-130">Common requests</span></span>

<span data-ttu-id="0d909-131">下表列出了可用于此 API 的一些常见请求。</span><span class="sxs-lookup"><span data-stu-id="0d909-131">The following table lists some common requests that you can use with this API.</span></span>

| <span data-ttu-id="0d909-132">Operation</span><span class="sxs-lookup"><span data-stu-id="0d909-132">Operation</span></span> | <span data-ttu-id="0d909-133">在 Graph 浏览器中试用</span><span class="sxs-lookup"><span data-stu-id="0d909-133">Try in Graph Explorer</span></span> | <span data-ttu-id="0d909-134">说明</span><span class="sxs-lookup"><span data-stu-id="0d909-134">Description</span></span> |
| --------- | --- | ----------- |
| [<span data-ttu-id="0d909-135">getCredentialUserRegistrationcount</span><span class="sxs-lookup"><span data-stu-id="0d909-135">getCredentialUserRegistrationcount</span></span>](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta&preserve-view=true) | <span data-ttu-id="0d909-136">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span><span class="sxs-lookup"><span data-stu-id="0d909-136">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span></span> | <span data-ttu-id="0d909-137">获取注册自助密码重置和 MFA 的用户数。</span><span class="sxs-lookup"><span data-stu-id="0d909-137">Get the number of users registered for self-service password reset and MFA.</span></span> |
| [<span data-ttu-id="0d909-138">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="0d909-138">getCredentialUsageSummary</span></span>](/graph/api/resources/credentialusagesummary?view=graph-rest-beta&preserve-view=true) | [<span data-ttu-id="0d909-139">GET /credentialusagesummary</span><span class="sxs-lookup"><span data-stu-id="0d909-139">GET /credentialusagesummary</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | <span data-ttu-id="0d909-140">获取使用自助服务密码重置的用户数。</span><span class="sxs-lookup"><span data-stu-id="0d909-140">Get the number of users using self-service password reset.</span></span> |
| [<span data-ttu-id="0d909-141">credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="0d909-141">credentialUserRegistrationDetails</span></span>](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta&preserve-view=true) | [<span data-ttu-id="0d909-142">GET /credentialuserregistrationdetails</span><span class="sxs-lookup"><span data-stu-id="0d909-142">GET /credentialuserregistrationdetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | <span data-ttu-id="0d909-143">获取自助服务密码重置和 MFA 注册活动的用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="0d909-143">Get the user details for self-service password reset and MFA registration activities.</span></span> |
| [<span data-ttu-id="0d909-144">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="0d909-144">userCredentialUsageDetails</span></span>](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta&preserve-view=true) | [<span data-ttu-id="0d909-145">GET /usercredentialusagedetails</span><span class="sxs-lookup"><span data-stu-id="0d909-145">GET /usercredentialusagedetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | <span data-ttu-id="0d909-146">获取所有自助式密码重置活动的用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="0d909-146">Get user details for all self-service password reset activities.</span></span> |
| [<span data-ttu-id="0d909-147">usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="0d909-147">usersRegisteredByFeature</span></span>](/graph/api/resources/userregistrationfeaturesummary?view=graph-rest-beta&preserve-view=true) | <span data-ttu-id="0d909-148">[GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta)</span><span class="sxs-lookup"><span data-stu-id="0d909-148">[GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta)</span></span> | <span data-ttu-id="0d909-149">获取能够进行多重身份验证、自助服务密码重置和无密码身份验证的用户数量。</span><span class="sxs-lookup"><span data-stu-id="0d909-149">Get the number of users capable of multi-factor authentication, self-service password reset and passwordless authentication.</span></span> |
| [<span data-ttu-id="0d909-150">usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="0d909-150">usersRegisteredByMethod</span></span>](/graph/api/resources/userregistrationmethodsummary?view=graph-rest-beta&preserve-view=true) | <span data-ttu-id="0d909-151">[GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta)</span><span class="sxs-lookup"><span data-stu-id="0d909-151">[GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta)</span></span> | <span data-ttu-id="0d909-152">获取每个身份验证方法注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="0d909-152">Get the number of users registered for each authentication method.</span></span> |

## <a name="next-steps"></a><span data-ttu-id="0d909-153">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0d909-153">Next steps</span></span>

- <span data-ttu-id="0d909-154">了解如何部署 [Azure Active Directory 自助服务密码重置](/azure/active-directory/authentication/howto-sspr-deployment)。</span><span class="sxs-lookup"><span data-stu-id="0d909-154">Learn how to [deploy Azure Active Directory self-service password reset](/azure/active-directory/authentication/howto-sspr-deployment).</span></span>
- <span data-ttu-id="0d909-155">了解如何部署[Azure Active Directory MFA。](/azure/active-directory/authentication/howto-mfa-getstarted)</span><span class="sxs-lookup"><span data-stu-id="0d909-155">Learn how to deploy [Azure Active Directory MFA](/azure/active-directory/authentication/howto-mfa-getstarted).</span></span>
- <span data-ttu-id="0d909-156">了解如何启用组合 [安全信息注册](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)。</span><span class="sxs-lookup"><span data-stu-id="0d909-156">Learn how to enable [combined security info registration](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span></span>
