---
title: signIn 资源类型
description: 详细介绍租户 (目录) 的用户和应用程序登录活动。
author: khotz
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fd8981e527bfa8d480dc0e9cda23a061fb9c5ac2
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673873"
---
# <a name="signin-resource-type"></a><span data-ttu-id="0c3cc-103">signIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c3cc-103">signIn resource type</span></span>

<span data-ttu-id="0c3cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c3cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c3cc-105">详细介绍租户 (目录) 的用户和应用程序登录活动。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-105">Details user and application sign-in activity for a tenant (directory).</span></span>

## <a name="methods"></a><span data-ttu-id="0c3cc-106">方法</span><span class="sxs-lookup"><span data-stu-id="0c3cc-106">Methods</span></span>

| <span data-ttu-id="0c3cc-107">方法</span><span class="sxs-lookup"><span data-stu-id="0c3cc-107">Method</span></span>           | <span data-ttu-id="0c3cc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0c3cc-108">Return Type</span></span>    |<span data-ttu-id="0c3cc-109">说明</span><span class="sxs-lookup"><span data-stu-id="0c3cc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c3cc-110">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="0c3cc-110">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="0c3cc-111">signIn</span><span class="sxs-lookup"><span data-stu-id="0c3cc-111">signIn</span></span>](signin.md) |<span data-ttu-id="0c3cc-112">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-112">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="0c3cc-113">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="0c3cc-113">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="0c3cc-114">signIn</span><span class="sxs-lookup"><span data-stu-id="0c3cc-114">signIn</span></span>](signin.md) |<span data-ttu-id="0c3cc-115">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-115">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c3cc-116">属性</span><span class="sxs-lookup"><span data-stu-id="0c3cc-116">Properties</span></span>
| <span data-ttu-id="0c3cc-117">属性</span><span class="sxs-lookup"><span data-stu-id="0c3cc-117">Property</span></span>     | <span data-ttu-id="0c3cc-118">类型</span><span class="sxs-lookup"><span data-stu-id="0c3cc-118">Type</span></span>   |<span data-ttu-id="0c3cc-119">说明</span><span class="sxs-lookup"><span data-stu-id="0c3cc-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c3cc-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c3cc-120">appDisplayName</span></span>|<span data-ttu-id="0c3cc-121">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-121">String</span></span>|<span data-ttu-id="0c3cc-122">Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-122">App name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="0c3cc-123">appId</span><span class="sxs-lookup"><span data-stu-id="0c3cc-123">appId</span></span>|<span data-ttu-id="0c3cc-124">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-124">String</span></span>|<span data-ttu-id="0c3cc-125">表示 Azure Active Directory 中的应用程序 ID 的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-125">Unique GUID representing the app ID in the Azure Active Directory.</span></span>|
|<span data-ttu-id="0c3cc-126">appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0c3cc-126">appliedConditionalAccessPolicy</span></span>|<span data-ttu-id="0c3cc-127">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c3cc-127">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection</span></span>|<span data-ttu-id="0c3cc-128">提供由相应登录活动触发的条件访问策略列表。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-128">Provides a list of conditional access policies that are triggered by the corresponding sign-in activity.</span></span>|
|<span data-ttu-id="0c3cc-129">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="0c3cc-129">clientAppUsed</span></span>|<span data-ttu-id="0c3cc-130">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-130">String</span></span>|<span data-ttu-id="0c3cc-131">标识用于登录活动的旧客户端。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-131">Identifies the legacy client used for sign-in activity.</span></span>  <span data-ttu-id="0c3cc-132">包括浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI、SMTP 和 POP。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-132">Includes Browser, Exchange Active Sync, modern clients, IMAP, MAPI, SMTP, and POP.</span></span>|
|<span data-ttu-id="0c3cc-133">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="0c3cc-133">conditionalAccessStatus</span></span>|<span data-ttu-id="0c3cc-134">string</span><span class="sxs-lookup"><span data-stu-id="0c3cc-134">string</span></span>| <span data-ttu-id="0c3cc-135">报告激活的条件访问策略的状态。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-135">Reports status of an activated conditional access policy.</span></span> <span data-ttu-id="0c3cc-136">可能的值是： `success` 、 `failure` 、 `notApplied` 和 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-136">Possible values are: `success`, `failure`, `notApplied`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0c3cc-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="0c3cc-137">correlationId</span></span>|<span data-ttu-id="0c3cc-138">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-138">String</span></span>|<span data-ttu-id="0c3cc-139">启动登录时从客户端发送的请求 ID;用于对登录活动进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-139">The request ID sent from the client when the sign-in is initiated; used to troubleshoot sign-in activity.</span></span>|
|<span data-ttu-id="0c3cc-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c3cc-140">createdDateTime</span></span>|<span data-ttu-id="0c3cc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c3cc-141">DateTimeOffset</span></span>|<span data-ttu-id="0c3cc-142">启动登录) 日期和时间 (UTC。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-142">Date and time (UTC) the sign-in was initiated.</span></span> <span data-ttu-id="0c3cc-143">示例：2014年1月1日午夜，报告为 `'2014-01-01T00:00:00Z'` 。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-143">Example: midnight on Jan 1, 2014 is reported as `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0c3cc-144">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="0c3cc-144">deviceDetail</span></span>|[<span data-ttu-id="0c3cc-145">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="0c3cc-145">deviceDetail</span></span>](devicedetail.md)|<span data-ttu-id="0c3cc-146">发生登录的设备信息;包括设备 ID、操作系统和浏览器。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-146">Device information from where the sign-in occurred; includes device ID, operating system, and browser.</span></span> |
|<span data-ttu-id="0c3cc-147">id</span><span class="sxs-lookup"><span data-stu-id="0c3cc-147">id</span></span>|<span data-ttu-id="0c3cc-148">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-148">String</span></span>|<span data-ttu-id="0c3cc-149">表示登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-149">Unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="0c3cc-150">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0c3cc-150">ipAddress</span></span>|<span data-ttu-id="0c3cc-151">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-151">String</span></span>|<span data-ttu-id="0c3cc-152">用于登录的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-152">IP address of the client used to sign in.</span></span>|
|<span data-ttu-id="0c3cc-153">isInteractive</span><span class="sxs-lookup"><span data-stu-id="0c3cc-153">isInteractive</span></span>|<span data-ttu-id="0c3cc-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c3cc-154">Boolean</span></span>|<span data-ttu-id="0c3cc-155">指示登录是否为交互式登录。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-155">Indicates if a sign-in is interactive or not.</span></span>|
|<span data-ttu-id="0c3cc-156">location</span><span class="sxs-lookup"><span data-stu-id="0c3cc-156">location</span></span>|[<span data-ttu-id="0c3cc-157">signInLocation</span><span class="sxs-lookup"><span data-stu-id="0c3cc-157">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="0c3cc-158">提供登录所源于的城市、州和国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-158">Provides the city, state, and country code where the sign-in originated.</span></span>|
|<span data-ttu-id="0c3cc-159">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c3cc-159">resourceDisplayName</span></span>|<span data-ttu-id="0c3cc-160">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-160">String</span></span>|<span data-ttu-id="0c3cc-161">用户登录到的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-161">Name of the resource the user signed into.</span></span>|
|<span data-ttu-id="0c3cc-162">resourceId</span><span class="sxs-lookup"><span data-stu-id="0c3cc-162">resourceId</span></span>|<span data-ttu-id="0c3cc-163">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-163">String</span></span>|<span data-ttu-id="0c3cc-164">用户登录到的资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-164">ID of the resource that the user signed into.</span></span>|
|<span data-ttu-id="0c3cc-165">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0c3cc-165">riskDetail</span></span>|<span data-ttu-id="0c3cc-166">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0c3cc-166">riskDetail</span></span>|<span data-ttu-id="0c3cc-167">提供风险用户、登录或风险事件的特定状态背后的“原因”。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-167">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="0c3cc-168">可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-168">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="0c3cc-169">值 `none` 表示到目前为止尚未对用户或登录执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-169">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> <br><span data-ttu-id="0c3cc-170">**注意：** 此属性的详细信息需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-170">**Note:** Details for this property require an Azure AD Premium P2 license.</span></span> <span data-ttu-id="0c3cc-171">其他许可证返回值 `hidden` 。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-171">Other licenses return the value `hidden`.</span></span>|
|<span data-ttu-id="0c3cc-172">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="0c3cc-172">riskEventTypes</span></span>|<span data-ttu-id="0c3cc-173">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="0c3cc-173">riskEventType collection</span></span>|<span data-ttu-id="0c3cc-174">与登录相关联的风险事件类型。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-174">Risk event types associated with the sign-in.</span></span> <span data-ttu-id="0c3cc-175">可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-175">The possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0c3cc-176">riskEventTypes_v2</span><span class="sxs-lookup"><span data-stu-id="0c3cc-176">riskEventTypes_v2</span></span>|<span data-ttu-id="0c3cc-177">String collection</span><span class="sxs-lookup"><span data-stu-id="0c3cc-177">String collection</span></span>|<span data-ttu-id="0c3cc-178">与登录相关联的风险事件类型的列表。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-178">The list of risk event types associated with the sign-in.</span></span> <span data-ttu-id="0c3cc-179">可能的值：、、、、、、、、、 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` 或 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-179">Possible values: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, or `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0c3cc-180">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="0c3cc-180">riskLevelAggregated</span></span>|<span data-ttu-id="0c3cc-181">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0c3cc-181">riskLevel</span></span>|<span data-ttu-id="0c3cc-182">聚合风险级别。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-182">Aggregated risk level.</span></span> <span data-ttu-id="0c3cc-183">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-183">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="0c3cc-184">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-184">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="0c3cc-185">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-185">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="0c3cc-186">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-186">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="0c3cc-187">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="0c3cc-187">riskLevelDuringSignIn</span></span>|<span data-ttu-id="0c3cc-188">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0c3cc-188">riskLevel</span></span>|<span data-ttu-id="0c3cc-189">登录过程中的风险级别。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-189">Risk level during sign-in.</span></span> <span data-ttu-id="0c3cc-190">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-190">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="0c3cc-191">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-191">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="0c3cc-192">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-192">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="0c3cc-193">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-193">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="0c3cc-194">riskState</span><span class="sxs-lookup"><span data-stu-id="0c3cc-194">riskState</span></span>|<span data-ttu-id="0c3cc-195">riskState</span><span class="sxs-lookup"><span data-stu-id="0c3cc-195">riskState</span></span>|<span data-ttu-id="0c3cc-196">报告有风险的用户、登录或风险事件的状态。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-196">Reports status of the risky user, sign-in, or a risk event.</span></span> <span data-ttu-id="0c3cc-197">可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-197">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0c3cc-198">status</span><span class="sxs-lookup"><span data-stu-id="0c3cc-198">status</span></span>|[<span data-ttu-id="0c3cc-199">signInStatus</span><span class="sxs-lookup"><span data-stu-id="0c3cc-199">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="0c3cc-200">登录状态。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-200">Sign-in status.</span></span> <span data-ttu-id="0c3cc-201">可取值包括 `Success` 和 `Failure`。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-201">Possible values include `Success` and `Failure`.</span></span>|
|<span data-ttu-id="0c3cc-202">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c3cc-202">userDisplayName</span></span>|<span data-ttu-id="0c3cc-203">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-203">String</span></span>|<span data-ttu-id="0c3cc-204">启动登录的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-204">Display name of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="0c3cc-205">userId</span><span class="sxs-lookup"><span data-stu-id="0c3cc-205">userId</span></span>|<span data-ttu-id="0c3cc-206">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-206">String</span></span>|<span data-ttu-id="0c3cc-207">启动登录的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-207">ID of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="0c3cc-208">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c3cc-208">userPrincipalName</span></span>|<span data-ttu-id="0c3cc-209">String</span><span class="sxs-lookup"><span data-stu-id="0c3cc-209">String</span></span>|<span data-ttu-id="0c3cc-210">启动登录的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-210">User principal name of the user that initiated the sign-in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c3cc-211">关系</span><span class="sxs-lookup"><span data-stu-id="0c3cc-211">Relationships</span></span>

<span data-ttu-id="0c3cc-212">无</span><span class="sxs-lookup"><span data-stu-id="0c3cc-212">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0c3cc-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c3cc-213">JSON representation</span></span>

<span data-ttu-id="0c3cc-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c3cc-214">Here is a JSON representation of the resource.</span></span>

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
