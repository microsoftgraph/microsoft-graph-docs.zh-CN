---
title: signIn 资源类型
description: 详细介绍租户（目录）的用户和应用程序登录活动。
author: kholtz
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b9be21b34b291d4a4c7278242c56a3cf63c2c7ea
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124803"
---
# <a name="signin-resource-type"></a><span data-ttu-id="ffb8c-103">signIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffb8c-103">signIn resource type</span></span>

<span data-ttu-id="ffb8c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffb8c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffb8c-105">详细介绍租户（目录）的用户和应用程序登录活动。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-105">Details user and application sign-in activity for a tenant (directory).</span></span>

## <a name="methods"></a><span data-ttu-id="ffb8c-106">方法</span><span class="sxs-lookup"><span data-stu-id="ffb8c-106">Methods</span></span>

| <span data-ttu-id="ffb8c-107">方法</span><span class="sxs-lookup"><span data-stu-id="ffb8c-107">Method</span></span>           | <span data-ttu-id="ffb8c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ffb8c-108">Return Type</span></span>    |<span data-ttu-id="ffb8c-109">说明</span><span class="sxs-lookup"><span data-stu-id="ffb8c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ffb8c-110">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="ffb8c-110">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="ffb8c-111">signIn</span><span class="sxs-lookup"><span data-stu-id="ffb8c-111">signIn</span></span>](signin.md) |<span data-ttu-id="ffb8c-112">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-112">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="ffb8c-113">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="ffb8c-113">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="ffb8c-114">signIn</span><span class="sxs-lookup"><span data-stu-id="ffb8c-114">signIn</span></span>](signin.md) |<span data-ttu-id="ffb8c-115">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-115">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ffb8c-116">属性</span><span class="sxs-lookup"><span data-stu-id="ffb8c-116">Properties</span></span>
| <span data-ttu-id="ffb8c-117">属性</span><span class="sxs-lookup"><span data-stu-id="ffb8c-117">Property</span></span>     | <span data-ttu-id="ffb8c-118">类型</span><span class="sxs-lookup"><span data-stu-id="ffb8c-118">Type</span></span>   |<span data-ttu-id="ffb8c-119">说明</span><span class="sxs-lookup"><span data-stu-id="ffb8c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffb8c-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="ffb8c-120">appDisplayName</span></span>|<span data-ttu-id="ffb8c-121">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-121">String</span></span>|<span data-ttu-id="ffb8c-122">Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-122">App name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="ffb8c-123">appId</span><span class="sxs-lookup"><span data-stu-id="ffb8c-123">appId</span></span>|<span data-ttu-id="ffb8c-124">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-124">String</span></span>|<span data-ttu-id="ffb8c-125">表示 Azure Active Directory 中的应用程序 ID 的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-125">Unique GUID representing the app ID in the Azure Active Directory.</span></span>|
|<span data-ttu-id="ffb8c-126">appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ffb8c-126">appliedConditionalAccessPolicy</span></span>|<span data-ttu-id="ffb8c-127">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffb8c-127">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection</span></span>|<span data-ttu-id="ffb8c-128">提供由相应登录活动触发的条件访问策略列表。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-128">Provides a list of conditional access policies that are triggered by the corresponding sign-in activity.</span></span>|
|<span data-ttu-id="ffb8c-129">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="ffb8c-129">clientAppUsed</span></span>|<span data-ttu-id="ffb8c-130">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-130">String</span></span>|<span data-ttu-id="ffb8c-131">标识用于登录活动的旧客户端。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-131">Identifies the legacy client used for sign-in activity.</span></span>  <span data-ttu-id="ffb8c-132">包括浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI、SMTP 和 POP。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-132">Includes Browser, Exchange Active Sync, modern clients, IMAP, MAPI, SMTP, and POP.</span></span>|
|<span data-ttu-id="ffb8c-133">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="ffb8c-133">conditionalAccessStatus</span></span>|<span data-ttu-id="ffb8c-134">string</span><span class="sxs-lookup"><span data-stu-id="ffb8c-134">string</span></span>| <span data-ttu-id="ffb8c-135">报告激活的条件访问策略的状态。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-135">Reports status of an activated conditional access policy.</span></span> <span data-ttu-id="ffb8c-136">可能的值是`success`： `failure`、 `notApplied`、和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-136">Possible values are: `success`, `failure`, `notApplied`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ffb8c-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="ffb8c-137">correlationId</span></span>|<span data-ttu-id="ffb8c-138">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-138">String</span></span>|<span data-ttu-id="ffb8c-139">启动登录时从客户端发送的请求 ID;用于对登录活动进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-139">The request ID sent from the client when the sign-in is initiated; used to troubleshoot sign-in activity.</span></span>|
|<span data-ttu-id="ffb8c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb8c-140">createdDateTime</span></span>|<span data-ttu-id="ffb8c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb8c-141">DateTimeOffset</span></span>|<span data-ttu-id="ffb8c-142">启动登录的日期和时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-142">Date and time (UTC) the sign-in was initiated.</span></span> <span data-ttu-id="ffb8c-143">示例：2014年1月1日午夜，报告`'2014-01-01T00:00:00Z'`为。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-143">Example: midnight on Jan 1, 2014 is reported as `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ffb8c-144">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="ffb8c-144">deviceDetail</span></span>|[<span data-ttu-id="ffb8c-145">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="ffb8c-145">deviceDetail</span></span>](devicedetail.md)|<span data-ttu-id="ffb8c-146">发生登录的设备信息;包括设备 ID、操作系统和浏览器。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-146">Device information from where the sign-in occurred; includes device ID, operating system, and browser.</span></span> |
|<span data-ttu-id="ffb8c-147">id</span><span class="sxs-lookup"><span data-stu-id="ffb8c-147">id</span></span>|<span data-ttu-id="ffb8c-148">字符串</span><span class="sxs-lookup"><span data-stu-id="ffb8c-148">String</span></span>|<span data-ttu-id="ffb8c-149">表示登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-149">Unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="ffb8c-150">ipAddress</span><span class="sxs-lookup"><span data-stu-id="ffb8c-150">ipAddress</span></span>|<span data-ttu-id="ffb8c-151">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-151">String</span></span>|<span data-ttu-id="ffb8c-152">用于登录的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-152">IP address of the client used to sign in.</span></span>|
|<span data-ttu-id="ffb8c-153">isInteractive</span><span class="sxs-lookup"><span data-stu-id="ffb8c-153">isInteractive</span></span>|<span data-ttu-id="ffb8c-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffb8c-154">Boolean</span></span>|<span data-ttu-id="ffb8c-155">指示登录是否为交互式登录。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-155">Indicates if a sign-in is interactive or not.</span></span>|
|<span data-ttu-id="ffb8c-156">location</span><span class="sxs-lookup"><span data-stu-id="ffb8c-156">location</span></span>|[<span data-ttu-id="ffb8c-157">signInLocation</span><span class="sxs-lookup"><span data-stu-id="ffb8c-157">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="ffb8c-158">提供登录所源于的城市、州和国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-158">Provides the city, state, and country code where the sign-in originated.</span></span>|
|<span data-ttu-id="ffb8c-159">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ffb8c-159">resourceDisplayName</span></span>|<span data-ttu-id="ffb8c-160">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-160">String</span></span>|<span data-ttu-id="ffb8c-161">用户登录到的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-161">Name of the resource the user signed into.</span></span>|
|<span data-ttu-id="ffb8c-162">resourceId</span><span class="sxs-lookup"><span data-stu-id="ffb8c-162">resourceId</span></span>|<span data-ttu-id="ffb8c-163">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-163">String</span></span>|<span data-ttu-id="ffb8c-164">用户登录到的资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-164">ID of the resource that the user signed into.</span></span>|
|<span data-ttu-id="ffb8c-165">riskDetail</span><span class="sxs-lookup"><span data-stu-id="ffb8c-165">riskDetail</span></span>|<span data-ttu-id="ffb8c-166">riskDetail</span><span class="sxs-lookup"><span data-stu-id="ffb8c-166">riskDetail</span></span>|<span data-ttu-id="ffb8c-167">提供风险用户、登录或风险事件的特定状态背后的“原因”。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-167">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="ffb8c-168">可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-168">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="ffb8c-169">值 `none` 表示到目前为止尚未对用户或登录执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-169">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> <br><span data-ttu-id="ffb8c-170">**注意：** 此属性的详细信息需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-170">**Note:** Details for this property require an Azure AD Premium P2 license.</span></span> <span data-ttu-id="ffb8c-171">其他许可证返回值`hidden`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-171">Other licenses return the value `hidden`.</span></span>|
|<span data-ttu-id="ffb8c-172">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="ffb8c-172">riskEventTypes</span></span>|<span data-ttu-id="ffb8c-173">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="ffb8c-173">riskEventType collection</span></span>|<span data-ttu-id="ffb8c-174">与登录相关联的风险事件类型。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-174">Risk event types associated with the sign-in.</span></span> <span data-ttu-id="ffb8c-175">可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-175">The possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ffb8c-176">riskEventTypes_v2</span><span class="sxs-lookup"><span data-stu-id="ffb8c-176">riskEventTypes_v2</span></span>|<span data-ttu-id="ffb8c-177">String collection</span><span class="sxs-lookup"><span data-stu-id="ffb8c-177">String collection</span></span>|<span data-ttu-id="ffb8c-178">与登录相关联的风险事件类型的列表。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-178">The list of risk event types associated with the sign-in.</span></span> <span data-ttu-id="ffb8c-179">可能的值`unlikelyTravel`： `anonymizedIPAddress`、 `maliciousIPAddress`、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`、、、、、、、 `unknownFutureValue` `generic`或。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-179">Possible values: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, or `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ffb8c-180">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="ffb8c-180">riskLevelAggregated</span></span>|<span data-ttu-id="ffb8c-181">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ffb8c-181">riskLevel</span></span>|<span data-ttu-id="ffb8c-182">聚合风险级别。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-182">Aggregated risk level.</span></span> <span data-ttu-id="ffb8c-183">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-183">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="ffb8c-184">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-184">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="ffb8c-185">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-185">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="ffb8c-186">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-186">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="ffb8c-187">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="ffb8c-187">riskLevelDuringSignIn</span></span>|<span data-ttu-id="ffb8c-188">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ffb8c-188">riskLevel</span></span>|<span data-ttu-id="ffb8c-189">登录过程中的风险级别。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-189">Risk level during sign-in.</span></span> <span data-ttu-id="ffb8c-190">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-190">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="ffb8c-191">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-191">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="ffb8c-192">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-192">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="ffb8c-193">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-193">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="ffb8c-194">riskState</span><span class="sxs-lookup"><span data-stu-id="ffb8c-194">riskState</span></span>|<span data-ttu-id="ffb8c-195">riskState</span><span class="sxs-lookup"><span data-stu-id="ffb8c-195">riskState</span></span>|<span data-ttu-id="ffb8c-196">报告有风险的用户、登录或风险事件的状态。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-196">Reports status of the risky user, sign-in, or a risk event.</span></span> <span data-ttu-id="ffb8c-197">可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-197">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ffb8c-198">status</span><span class="sxs-lookup"><span data-stu-id="ffb8c-198">status</span></span>|[<span data-ttu-id="ffb8c-199">signInStatus</span><span class="sxs-lookup"><span data-stu-id="ffb8c-199">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="ffb8c-200">登录状态。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-200">Sign-in status.</span></span> <span data-ttu-id="ffb8c-201">可取值包括 `Success` 和 `Failure`。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-201">Possible values include `Success` and `Failure`.</span></span>|
|<span data-ttu-id="ffb8c-202">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ffb8c-202">userDisplayName</span></span>|<span data-ttu-id="ffb8c-203">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-203">String</span></span>|<span data-ttu-id="ffb8c-204">启动登录的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-204">Display name of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="ffb8c-205">userId</span><span class="sxs-lookup"><span data-stu-id="ffb8c-205">userId</span></span>|<span data-ttu-id="ffb8c-206">String</span><span class="sxs-lookup"><span data-stu-id="ffb8c-206">String</span></span>|<span data-ttu-id="ffb8c-207">启动登录的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-207">ID of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="ffb8c-208">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ffb8c-208">userPrincipalName</span></span>|<span data-ttu-id="ffb8c-209">字符串</span><span class="sxs-lookup"><span data-stu-id="ffb8c-209">String</span></span>|<span data-ttu-id="ffb8c-210">启动登录的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-210">User principal name of the user that initiated the sign-in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffb8c-211">关系</span><span class="sxs-lookup"><span data-stu-id="ffb8c-211">Relationships</span></span>

<span data-ttu-id="ffb8c-212">无</span><span class="sxs-lookup"><span data-stu-id="ffb8c-212">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ffb8c-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffb8c-213">JSON representation</span></span>

<span data-ttu-id="ffb8c-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffb8c-214">Here is a JSON representation of the resource.</span></span>

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
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "isInteractive": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["string"],
  "riskEventTypes_v2": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
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
