---
title: signIn 资源类型
doc_type: resourcePageType
description: 描述 Microsoft Graph API (REST) 的 signIn 资源，这有利于审核用户和应用程序登录活动（beta 版本）。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a0f3977c14ce8e0e53cdbd296ea28c4b79f5762
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396742"
---
# <a name="signin-resource-type"></a><span data-ttu-id="8548e-103">signIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="8548e-103">signIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8548e-104">提供有关目录中用户或应用程序登录活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8548e-104">Provides details about user or application sign-in activity in your directory.</span></span> 

## <a name="methods"></a><span data-ttu-id="8548e-105">方法</span><span class="sxs-lookup"><span data-stu-id="8548e-105">Methods</span></span>

| <span data-ttu-id="8548e-106">方法</span><span class="sxs-lookup"><span data-stu-id="8548e-106">Method</span></span>           | <span data-ttu-id="8548e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8548e-107">Return Type</span></span>    |<span data-ttu-id="8548e-108">说明</span><span class="sxs-lookup"><span data-stu-id="8548e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8548e-109">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="8548e-109">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="8548e-110">signIn</span><span class="sxs-lookup"><span data-stu-id="8548e-110">signIn</span></span>](signin.md) |<span data-ttu-id="8548e-111">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8548e-111">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="8548e-112">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="8548e-112">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="8548e-113">signIn</span><span class="sxs-lookup"><span data-stu-id="8548e-113">signIn</span></span>](signin.md) |<span data-ttu-id="8548e-114">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8548e-114">Read properties and relationships of a signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8548e-115">属性</span><span class="sxs-lookup"><span data-stu-id="8548e-115">Properties</span></span>
| <span data-ttu-id="8548e-116">属性</span><span class="sxs-lookup"><span data-stu-id="8548e-116">Property</span></span>     | <span data-ttu-id="8548e-117">类型</span><span class="sxs-lookup"><span data-stu-id="8548e-117">Type</span></span>   |<span data-ttu-id="8548e-118">说明</span><span class="sxs-lookup"><span data-stu-id="8548e-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8548e-119">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="8548e-119">appDisplayName</span></span>|<span data-ttu-id="8548e-120">String</span><span class="sxs-lookup"><span data-stu-id="8548e-120">String</span></span>|<span data-ttu-id="8548e-121">表示 Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="8548e-121">Refers to the application name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="8548e-122">appId</span><span class="sxs-lookup"><span data-stu-id="8548e-122">appId</span></span>|<span data-ttu-id="8548e-123">String</span><span class="sxs-lookup"><span data-stu-id="8548e-123">String</span></span>|<span data-ttu-id="8548e-124">表示唯一 GUID（表示 Azure Active Directory 中的应用程序 ID）。</span><span class="sxs-lookup"><span data-stu-id="8548e-124">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="8548e-125">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="8548e-125">clientAppUsed</span></span>|<span data-ttu-id="8548e-126">String</span><span class="sxs-lookup"><span data-stu-id="8548e-126">String</span></span>|<span data-ttu-id="8548e-127">提供用于登录活动的旧版客户端。例如，</span><span class="sxs-lookup"><span data-stu-id="8548e-127">Provides the legacy client used for sign-in activty.E.g.</span></span> <span data-ttu-id="8548e-128">包括浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI SMTP、POP。</span><span class="sxs-lookup"><span data-stu-id="8548e-128">includes Browser, Exchange Active Sync,Modern clients, IMAP, MAPI, SMTP, POP.</span></span>|
|<span data-ttu-id="8548e-129">appliedConditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="8548e-129">appliedConditionalAccessPolicies</span></span>|<span data-ttu-id="8548e-130">[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8548e-130">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span>|<span data-ttu-id="8548e-131">提供由相应登录活动触发的条件访问策略列表。</span><span class="sxs-lookup"><span data-stu-id="8548e-131">Provides a list of conditional access policies that are triggered by the corresponding sign-in activity.</span></span>|
|<span data-ttu-id="8548e-132">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="8548e-132">conditionalAccessStatus</span></span>|<span data-ttu-id="8548e-133">string</span><span class="sxs-lookup"><span data-stu-id="8548e-133">string</span></span>| <span data-ttu-id="8548e-134">提供触发的条件访问策略的状态。</span><span class="sxs-lookup"><span data-stu-id="8548e-134">Provides the status of the conditional access policy triggered.</span></span> <span data-ttu-id="8548e-135">可取值为：`success`、`failure`、`notApplied`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8548e-135">Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8548e-136">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="8548e-136">originalRequestId</span></span>|<span data-ttu-id="8548e-137">String</span><span class="sxs-lookup"><span data-stu-id="8548e-137">String</span></span>|<span data-ttu-id="8548e-138">身份验证序列中第一个请求的请求 ID。</span><span class="sxs-lookup"><span data-stu-id="8548e-138">The request id of the first request in the authentication sequence.</span></span>|
|<span data-ttu-id="8548e-139">isInteractive</span><span class="sxs-lookup"><span data-stu-id="8548e-139">isInteractive</span></span>|<span data-ttu-id="8548e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8548e-140">Boolean</span></span>|<span data-ttu-id="8548e-141">指示登录是否为交互式。</span><span class="sxs-lookup"><span data-stu-id="8548e-141">Indicates if a signIn is interactive or not.</span></span>|
|<span data-ttu-id="8548e-142">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="8548e-142">tokenIssuerName</span></span>|<span data-ttu-id="8548e-143">String</span><span class="sxs-lookup"><span data-stu-id="8548e-143">String</span></span>|<span data-ttu-id="8548e-144">标识提供者（例如 sts.microsoft.com）的名称</span><span class="sxs-lookup"><span data-stu-id="8548e-144">Name of the identity Provider (e.g. sts.microsoft.com)</span></span>|
|<span data-ttu-id="8548e-145">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="8548e-145">tokenIssuerType</span></span>|<span data-ttu-id="8548e-146">String</span><span class="sxs-lookup"><span data-stu-id="8548e-146">String</span></span>|<span data-ttu-id="8548e-147">提供标识提供者的类型。</span><span class="sxs-lookup"><span data-stu-id="8548e-147">Provides the type of identityProvider.</span></span> <span data-ttu-id="8548e-148">可取值为 `AzureAD`、`ADFederationServices`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8548e-148">Possible values are `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="8548e-149">correlationId</span><span class="sxs-lookup"><span data-stu-id="8548e-149">correlationId</span></span>|<span data-ttu-id="8548e-150">String</span><span class="sxs-lookup"><span data-stu-id="8548e-150">String</span></span>|<span data-ttu-id="8548e-151">表示登录启动时从客户端发送的 ID。</span><span class="sxs-lookup"><span data-stu-id="8548e-151">Refers to the ID that's sent from the client when the sign-in is initiated.</span></span> <span data-ttu-id="8548e-152">此属性用于在调用帮助台或支持时对相应的登录活动进行故障诊断。</span><span class="sxs-lookup"><span data-stu-id="8548e-152">This is used for troubleshooting the corresponding sign-in activity when calling helpdesk or support.</span></span>|
|<span data-ttu-id="8548e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8548e-153">createdDateTime</span></span>|<span data-ttu-id="8548e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8548e-154">DateTimeOffset</span></span>|<span data-ttu-id="8548e-155">提供登录启动的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8548e-155">Provides the date and time the sign-in was initiated.</span></span> <span data-ttu-id="8548e-156">时间戳类型始终为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8548e-156">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="8548e-157">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8548e-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8548e-158">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="8548e-158">deviceDetail</span></span>|[<span data-ttu-id="8548e-159">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="8548e-159">deviceDetail</span></span>](devicedetail.md)|<span data-ttu-id="8548e-160">提供发生登录的设备的信息。</span><span class="sxs-lookup"><span data-stu-id="8548e-160">Provides the device information from where the sign-in occurred.</span></span> <span data-ttu-id="8548e-161">包括设备 ID、操作系统、浏览器等信息。</span><span class="sxs-lookup"><span data-stu-id="8548e-161">It inclules information like deviceId, OS, browser.</span></span> |
|<span data-ttu-id="8548e-162">id</span><span class="sxs-lookup"><span data-stu-id="8548e-162">id</span></span>|<span data-ttu-id="8548e-163">String</span><span class="sxs-lookup"><span data-stu-id="8548e-163">String</span></span>|<span data-ttu-id="8548e-164">表示登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="8548e-164">Indicates unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="8548e-165">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8548e-165">ipAddress</span></span>|<span data-ttu-id="8548e-166">String</span><span class="sxs-lookup"><span data-stu-id="8548e-166">String</span></span>|<span data-ttu-id="8548e-167">提供发生登录的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="8548e-167">Provides the IP address of the client from where the sign-in occurred.</span></span>|
|<span data-ttu-id="8548e-168">location</span><span class="sxs-lookup"><span data-stu-id="8548e-168">location</span></span>|[<span data-ttu-id="8548e-169">signInLocation</span><span class="sxs-lookup"><span data-stu-id="8548e-169">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="8548e-170">提供发生登录的城市、省/市/自治区和 2 个字母的国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="8548e-170">Provides the city, state and 2 letter country code from where the sign-in occurred.</span></span>|
|<span data-ttu-id="8548e-171">processingTimeInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="8548e-171">processingTimeInMilliseconds</span></span>|<span data-ttu-id="8548e-172">Int</span><span class="sxs-lookup"><span data-stu-id="8548e-172">Int</span></span>|<span data-ttu-id="8548e-173">提供 AD STS 中的请求处理时间（以毫秒为单位）</span><span class="sxs-lookup"><span data-stu-id="8548e-173">Provides the request processing time in milliseconds in AD STS</span></span>|
|<span data-ttu-id="8548e-174">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8548e-174">riskDetail</span></span>|`riskDetail`|<span data-ttu-id="8548e-175">提供风险用户、登录或风险事件的特定状态背后的“原因”。</span><span class="sxs-lookup"><span data-stu-id="8548e-175">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="8548e-176">可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8548e-176">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="8548e-177">值 `none` 表示到目前为止尚未对用户或登录执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="8548e-177">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> <span data-ttu-id="8548e-178">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="8548e-178">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="8548e-179">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="8548e-179">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="8548e-180">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="8548e-180">riskLevelAggregated</span></span>|`riskLevel`|<span data-ttu-id="8548e-181">提供聚合的风险级别。</span><span class="sxs-lookup"><span data-stu-id="8548e-181">Provides the aggregated risk level.</span></span> <span data-ttu-id="8548e-182">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8548e-182">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="8548e-183">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="8548e-183">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="8548e-184">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="8548e-184">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="8548e-185">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="8548e-185">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="8548e-186">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="8548e-186">riskLevelDuringSignIn</span></span>|`riskLevel`|<span data-ttu-id="8548e-187">提供登录期间的风险级别。</span><span class="sxs-lookup"><span data-stu-id="8548e-187">Provides the risk level during sign-in.</span></span> <span data-ttu-id="8548e-188">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8548e-188">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="8548e-189">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="8548e-189">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="8548e-190">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="8548e-190">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="8548e-191">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="8548e-191">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="8548e-192">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="8548e-192">riskEventTypes</span></span>|<span data-ttu-id="8548e-193">`riskEventType` 集合</span><span class="sxs-lookup"><span data-stu-id="8548e-193">`riskEventType` collection</span></span>|<span data-ttu-id="8548e-194">提供与登录关联的风险事件类型列表。</span><span class="sxs-lookup"><span data-stu-id="8548e-194">Provides the list of risk event types associated with the sign-in.</span></span> <span data-ttu-id="8548e-195">可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8548e-195">The possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8548e-196">riskState</span><span class="sxs-lookup"><span data-stu-id="8548e-196">riskState</span></span>|`riskState`|<span data-ttu-id="8548e-197">提供风险用户、登录或风险事件的“风险状态”。</span><span class="sxs-lookup"><span data-stu-id="8548e-197">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="8548e-198">可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8548e-198">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8548e-199">mfaDetail</span><span class="sxs-lookup"><span data-stu-id="8548e-199">mfaDetail</span></span>|[<span data-ttu-id="8548e-200">mfaDetail</span><span class="sxs-lookup"><span data-stu-id="8548e-200">mfaDetail</span></span>](mfadetail.md)|<span data-ttu-id="8548e-201">提供相应登录的 MFA 相关信息，例如“需要 MFA”、“MFA 状态”。</span><span class="sxs-lookup"><span data-stu-id="8548e-201">Provides the MFA related information like MFA Required, MFA Status for the corresponding sign-in.</span></span>|
|<span data-ttu-id="8548e-202">networkLocationDetails</span><span class="sxs-lookup"><span data-stu-id="8548e-202">networkLocationDetails</span></span>|<span data-ttu-id="8548e-203">[networkLocationDetail](networklocationdetail.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8548e-203">[networkLocationDetail](networklocationdetail.md) collection</span></span>|<span data-ttu-id="8548e-204">提供有关网络位置的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8548e-204">Provides details about the network location.</span></span>|
|<span data-ttu-id="8548e-205">status</span><span class="sxs-lookup"><span data-stu-id="8548e-205">status</span></span>|[<span data-ttu-id="8548e-206">signInStatus</span><span class="sxs-lookup"><span data-stu-id="8548e-206">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="8548e-207">提供登录状态。</span><span class="sxs-lookup"><span data-stu-id="8548e-207">Provides the sign-in status.</span></span> <span data-ttu-id="8548e-208">可取值包括 `Success` 和 `Failure`。</span><span class="sxs-lookup"><span data-stu-id="8548e-208">Possible values include `Success` and `Failure`.</span></span>|
|<span data-ttu-id="8548e-209">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8548e-209">userDisplayName</span></span>|<span data-ttu-id="8548e-210">String</span><span class="sxs-lookup"><span data-stu-id="8548e-210">String</span></span>|<span data-ttu-id="8548e-211">指示用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8548e-211">Indicates the display Name of the User.</span></span>|
|<span data-ttu-id="8548e-212">userId</span><span class="sxs-lookup"><span data-stu-id="8548e-212">userId</span></span>|<span data-ttu-id="8548e-213">String</span><span class="sxs-lookup"><span data-stu-id="8548e-213">String</span></span>|<span data-ttu-id="8548e-214">指示用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="8548e-214">Indicates the userId of the user.</span></span>|
|<span data-ttu-id="8548e-215">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8548e-215">userPrincipalName</span></span>|<span data-ttu-id="8548e-216">String</span><span class="sxs-lookup"><span data-stu-id="8548e-216">String</span></span>|<span data-ttu-id="8548e-217">指示用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="8548e-217">Indicates the UPN of the user.</span></span>|
|<span data-ttu-id="8548e-218">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8548e-218">resourceDisplayName</span></span>|<span data-ttu-id="8548e-219">String</span><span class="sxs-lookup"><span data-stu-id="8548e-219">String</span></span>|<span data-ttu-id="8548e-220">指示用户登录的资源的名称</span><span class="sxs-lookup"><span data-stu-id="8548e-220">Indicates the name of the resource that the user signed into</span></span>|
|<span data-ttu-id="8548e-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="8548e-221">resourceId</span></span>|<span data-ttu-id="8548e-222">String</span><span class="sxs-lookup"><span data-stu-id="8548e-222">String</span></span>|<span data-ttu-id="8548e-223">指示用户登录的资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="8548e-223">Indicates the Id of the resource that the user signed into.</span></span>|
|<span data-ttu-id="8548e-224">authenticationMethodsUsed</span><span class="sxs-lookup"><span data-stu-id="8548e-224">authenticationMethodsUsed</span></span>|<span data-ttu-id="8548e-225">String</span><span class="sxs-lookup"><span data-stu-id="8548e-225">String</span></span>|<span data-ttu-id="8548e-226">指示使用的身份验证方法列表</span><span class="sxs-lookup"><span data-stu-id="8548e-226">Indicates the list of Authentication methods used</span></span>|

## <a name="relationships"></a><span data-ttu-id="8548e-227">关系</span><span class="sxs-lookup"><span data-stu-id="8548e-227">Relationships</span></span>
<span data-ttu-id="8548e-228">无</span><span class="sxs-lookup"><span data-stu-id="8548e-228">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8548e-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8548e-229">JSON representation</span></span>

<span data-ttu-id="8548e-230">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8548e-230">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signIn"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicies": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "originalRequestId": "String",
  "isInteractive": "String",
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "authenticationMethodsUsed": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "processingTimeInMilliseconds": 12356,
  "networkLocationDetails": [{"@odata.type": "microsoft.graph.networkLocationDetail"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
