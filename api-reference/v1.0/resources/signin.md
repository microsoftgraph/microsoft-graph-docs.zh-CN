---
title: signIn 资源类型
description: 详细介绍租户目录和租户 (登录) 。
author: besiler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76708c8515c27babf5dcf8cc0105a7c2cfd40f64
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784820"
---
# <a name="signin-resource-type"></a><span data-ttu-id="2a395-103">signIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a395-103">signIn resource type</span></span>

<span data-ttu-id="2a395-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a395-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a395-105">详细介绍租户目录和租户 (登录) 。</span><span class="sxs-lookup"><span data-stu-id="2a395-105">Details user and application sign-in activity for a tenant (directory).</span></span> <span data-ttu-id="2a395-106">你必须拥有 Azure AD Premium P1 或 P2 许可证才能使用 Microsoft Graph API 下载登录日志。</span><span class="sxs-lookup"><span data-stu-id="2a395-106">You must have an Azure AD Premium P1 or P2 license to download sign-in logs using the Microsoft Graph API.</span></span>

## <a name="methods"></a><span data-ttu-id="2a395-107">方法</span><span class="sxs-lookup"><span data-stu-id="2a395-107">Methods</span></span>

| <span data-ttu-id="2a395-108">方法</span><span class="sxs-lookup"><span data-stu-id="2a395-108">Method</span></span>           | <span data-ttu-id="2a395-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2a395-109">Return Type</span></span>    |<span data-ttu-id="2a395-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a395-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a395-111">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="2a395-111">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="2a395-112">signIn</span><span class="sxs-lookup"><span data-stu-id="2a395-112">signIn</span></span>](signin.md) |<span data-ttu-id="2a395-113">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2a395-113">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="2a395-114">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="2a395-114">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="2a395-115">signIn</span><span class="sxs-lookup"><span data-stu-id="2a395-115">signIn</span></span>](signin.md) |<span data-ttu-id="2a395-116">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2a395-116">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a395-117">属性</span><span class="sxs-lookup"><span data-stu-id="2a395-117">Properties</span></span>
| <span data-ttu-id="2a395-118">属性</span><span class="sxs-lookup"><span data-stu-id="2a395-118">Property</span></span>     | <span data-ttu-id="2a395-119">类型</span><span class="sxs-lookup"><span data-stu-id="2a395-119">Type</span></span>   |<span data-ttu-id="2a395-120">说明</span><span class="sxs-lookup"><span data-stu-id="2a395-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a395-121">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a395-121">appDisplayName</span></span>|<span data-ttu-id="2a395-122">String</span><span class="sxs-lookup"><span data-stu-id="2a395-122">String</span></span>|<span data-ttu-id="2a395-123">Azure 门户中显示的应用名称。</span><span class="sxs-lookup"><span data-stu-id="2a395-123">App name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="2a395-124">appId</span><span class="sxs-lookup"><span data-stu-id="2a395-124">appId</span></span>|<span data-ttu-id="2a395-125">String</span><span class="sxs-lookup"><span data-stu-id="2a395-125">String</span></span>|<span data-ttu-id="2a395-126">表示 Azure Active Directory 中的应用 ID 的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="2a395-126">Unique GUID representing the app ID in the Azure Active Directory.</span></span>|
|<span data-ttu-id="2a395-127">appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2a395-127">appliedConditionalAccessPolicy</span></span>|<span data-ttu-id="2a395-128">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2a395-128">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection</span></span>|<span data-ttu-id="2a395-129">提供由相应登录活动触发的条件访问策略列表。</span><span class="sxs-lookup"><span data-stu-id="2a395-129">Provides a list of conditional access policies that are triggered by the corresponding sign-in activity.</span></span>|
|<span data-ttu-id="2a395-130">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="2a395-130">clientAppUsed</span></span>|<span data-ttu-id="2a395-131">String</span><span class="sxs-lookup"><span data-stu-id="2a395-131">String</span></span>|<span data-ttu-id="2a395-132">标识用于登录活动的旧版客户端。</span><span class="sxs-lookup"><span data-stu-id="2a395-132">Identifies the legacy client used for sign-in activity.</span></span>  <span data-ttu-id="2a395-133">包括浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI、SMTP 和 POP。</span><span class="sxs-lookup"><span data-stu-id="2a395-133">Includes Browser, Exchange Active Sync, modern clients, IMAP, MAPI, SMTP, and POP.</span></span>|
|<span data-ttu-id="2a395-134">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="2a395-134">conditionalAccessStatus</span></span>|<span data-ttu-id="2a395-135">string</span><span class="sxs-lookup"><span data-stu-id="2a395-135">string</span></span>| <span data-ttu-id="2a395-136">报告激活的条件访问策略的状态。</span><span class="sxs-lookup"><span data-stu-id="2a395-136">Reports status of an activated conditional access policy.</span></span> <span data-ttu-id="2a395-137">可能的值是： `success` 、 `failure` 和 `notApplied` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="2a395-137">Possible values are: `success`, `failure`, `notApplied`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2a395-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="2a395-138">correlationId</span></span>|<span data-ttu-id="2a395-139">String</span><span class="sxs-lookup"><span data-stu-id="2a395-139">String</span></span>|<span data-ttu-id="2a395-140">启动登录时从客户端发送的请求 ID;用于排查登录活动故障。</span><span class="sxs-lookup"><span data-stu-id="2a395-140">The request ID sent from the client when the sign-in is initiated; used to troubleshoot sign-in activity.</span></span>|
|<span data-ttu-id="2a395-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a395-141">createdDateTime</span></span>|<span data-ttu-id="2a395-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a395-142">DateTimeOffset</span></span>|<span data-ttu-id="2a395-143">启动登录 (UTC) 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2a395-143">Date and time (UTC) the sign-in was initiated.</span></span> <span data-ttu-id="2a395-144">示例：2014 年 1 月 1 日午夜报告为 `'2014-01-01T00:00:00Z'` 。</span><span class="sxs-lookup"><span data-stu-id="2a395-144">Example: midnight on Jan 1, 2014 is reported as `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2a395-145">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="2a395-145">deviceDetail</span></span>|[<span data-ttu-id="2a395-146">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="2a395-146">deviceDetail</span></span>](devicedetail.md)|<span data-ttu-id="2a395-147">登录发生位置的设备信息;包括设备 ID、操作系统和浏览器。</span><span class="sxs-lookup"><span data-stu-id="2a395-147">Device information from where the sign-in occurred; includes device ID, operating system, and browser.</span></span> |
|<span data-ttu-id="2a395-148">id</span><span class="sxs-lookup"><span data-stu-id="2a395-148">id</span></span>|<span data-ttu-id="2a395-149">String</span><span class="sxs-lookup"><span data-stu-id="2a395-149">String</span></span>|<span data-ttu-id="2a395-150">表示登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2a395-150">Unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="2a395-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2a395-151">ipAddress</span></span>|<span data-ttu-id="2a395-152">String</span><span class="sxs-lookup"><span data-stu-id="2a395-152">String</span></span>|<span data-ttu-id="2a395-153">用于登录的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="2a395-153">IP address of the client used to sign in.</span></span>|
|<span data-ttu-id="2a395-154">isInteractive</span><span class="sxs-lookup"><span data-stu-id="2a395-154">isInteractive</span></span>|<span data-ttu-id="2a395-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a395-155">Boolean</span></span>|<span data-ttu-id="2a395-156">指示登录是否交互。</span><span class="sxs-lookup"><span data-stu-id="2a395-156">Indicates if a sign-in is interactive or not.</span></span>|
|<span data-ttu-id="2a395-157">location</span><span class="sxs-lookup"><span data-stu-id="2a395-157">location</span></span>|[<span data-ttu-id="2a395-158">signInLocation</span><span class="sxs-lookup"><span data-stu-id="2a395-158">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="2a395-159">提供登录来源城市、省/市/市/地区代码。</span><span class="sxs-lookup"><span data-stu-id="2a395-159">Provides the city, state, and country code where the sign-in originated.</span></span>|
|<span data-ttu-id="2a395-160">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a395-160">resourceDisplayName</span></span>|<span data-ttu-id="2a395-161">String</span><span class="sxs-lookup"><span data-stu-id="2a395-161">String</span></span>|<span data-ttu-id="2a395-162">用户登录的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="2a395-162">Name of the resource the user signed into.</span></span>|
|<span data-ttu-id="2a395-163">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a395-163">resourceId</span></span>|<span data-ttu-id="2a395-164">String</span><span class="sxs-lookup"><span data-stu-id="2a395-164">String</span></span>|<span data-ttu-id="2a395-165">用户登录的资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="2a395-165">ID of the resource that the user signed into.</span></span>|
|<span data-ttu-id="2a395-166">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2a395-166">riskDetail</span></span>|<span data-ttu-id="2a395-167">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2a395-167">riskDetail</span></span>|<span data-ttu-id="2a395-168">提供风险用户、登录或风险事件的特定状态背后的“原因”。</span><span class="sxs-lookup"><span data-stu-id="2a395-168">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="2a395-169">可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2a395-169">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="2a395-170">值 `none` 表示到目前为止尚未对用户或登录执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="2a395-170">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> <br><span data-ttu-id="2a395-171">**注意：** 此属性的详细信息需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="2a395-171">**Note:** Details for this property require an Azure AD Premium P2 license.</span></span> <span data-ttu-id="2a395-172">其他许可证返回值 `hidden` 。</span><span class="sxs-lookup"><span data-stu-id="2a395-172">Other licenses return the value `hidden`.</span></span>|
|<span data-ttu-id="2a395-173">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="2a395-173">riskEventTypes</span></span>|<span data-ttu-id="2a395-174">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="2a395-174">riskEventType collection</span></span>|<span data-ttu-id="2a395-175">与登录相关联的风险事件类型。</span><span class="sxs-lookup"><span data-stu-id="2a395-175">Risk event types associated with the sign-in.</span></span> <span data-ttu-id="2a395-176">可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2a395-176">The possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2a395-177">riskEventTypes_v2</span><span class="sxs-lookup"><span data-stu-id="2a395-177">riskEventTypes_v2</span></span>|<span data-ttu-id="2a395-178">String collection</span><span class="sxs-lookup"><span data-stu-id="2a395-178">String collection</span></span>|<span data-ttu-id="2a395-179">与登录相关联的风险事件类型列表。</span><span class="sxs-lookup"><span data-stu-id="2a395-179">The list of risk event types associated with the sign-in.</span></span> <span data-ttu-id="2a395-180">可能的值 `unlikelyTravel` ：、 `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` 或 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="2a395-180">Possible values: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, or `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2a395-181">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="2a395-181">riskLevelAggregated</span></span>|<span data-ttu-id="2a395-182">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2a395-182">riskLevel</span></span>|<span data-ttu-id="2a395-183">聚合风险级别。</span><span class="sxs-lookup"><span data-stu-id="2a395-183">Aggregated risk level.</span></span> <span data-ttu-id="2a395-184">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2a395-184">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="2a395-185">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="2a395-185">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="2a395-186">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="2a395-186">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="2a395-187">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="2a395-187">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="2a395-188">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="2a395-188">riskLevelDuringSignIn</span></span>|<span data-ttu-id="2a395-189">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2a395-189">riskLevel</span></span>|<span data-ttu-id="2a395-190">登录期间的风险级别。</span><span class="sxs-lookup"><span data-stu-id="2a395-190">Risk level during sign-in.</span></span> <span data-ttu-id="2a395-191">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2a395-191">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="2a395-192">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="2a395-192">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="2a395-193">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="2a395-193">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="2a395-194">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="2a395-194">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="2a395-195">riskState</span><span class="sxs-lookup"><span data-stu-id="2a395-195">riskState</span></span>|<span data-ttu-id="2a395-196">riskState</span><span class="sxs-lookup"><span data-stu-id="2a395-196">riskState</span></span>|<span data-ttu-id="2a395-197">报告风险用户、登录或风险事件的状态。</span><span class="sxs-lookup"><span data-stu-id="2a395-197">Reports status of the risky user, sign-in, or a risk event.</span></span> <span data-ttu-id="2a395-198">可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2a395-198">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2a395-199">status</span><span class="sxs-lookup"><span data-stu-id="2a395-199">status</span></span>|[<span data-ttu-id="2a395-200">signInStatus</span><span class="sxs-lookup"><span data-stu-id="2a395-200">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="2a395-201">登录状态。</span><span class="sxs-lookup"><span data-stu-id="2a395-201">Sign-in status.</span></span> <span data-ttu-id="2a395-202">包括错误代码和错误描述， (登录失败时返回) 。</span><span class="sxs-lookup"><span data-stu-id="2a395-202">Includes the error code and description of the error (in case of a sign-in failure).</span></span>|
|<span data-ttu-id="2a395-203">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a395-203">userDisplayName</span></span>|<span data-ttu-id="2a395-204">String</span><span class="sxs-lookup"><span data-stu-id="2a395-204">String</span></span>|<span data-ttu-id="2a395-205">启动登录的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2a395-205">Display name of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="2a395-206">userId</span><span class="sxs-lookup"><span data-stu-id="2a395-206">userId</span></span>|<span data-ttu-id="2a395-207">String</span><span class="sxs-lookup"><span data-stu-id="2a395-207">String</span></span>|<span data-ttu-id="2a395-208">启动登录的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="2a395-208">ID of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="2a395-209">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2a395-209">userPrincipalName</span></span>|<span data-ttu-id="2a395-210">String</span><span class="sxs-lookup"><span data-stu-id="2a395-210">String</span></span>|<span data-ttu-id="2a395-211">启动登录的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="2a395-211">User principal name of the user that initiated the sign-in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a395-212">关系</span><span class="sxs-lookup"><span data-stu-id="2a395-212">Relationships</span></span>

<span data-ttu-id="2a395-213">无</span><span class="sxs-lookup"><span data-stu-id="2a395-213">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2a395-214">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a395-214">JSON representation</span></span>

<span data-ttu-id="2a395-215">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a395-215">Here is a JSON representation of the resource.</span></span>

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

