---
title: signIn 资源类型
description: 详细介绍租户 (目录) 的用户和应用程序登录活动。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb73b843643c5ffba1b5cdac3d7fd519819109ba
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629241"
---
# <a name="signin-resource-type"></a><span data-ttu-id="c3f6b-103">signIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3f6b-103">signIn resource type</span></span>

<span data-ttu-id="c3f6b-104">详细介绍租户 (目录) 的用户和应用程序登录活动。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-104">Details user and application sign-in activity for a tenant (directory).</span></span>

## <a name="methods"></a><span data-ttu-id="c3f6b-105">方法</span><span class="sxs-lookup"><span data-stu-id="c3f6b-105">Methods</span></span>

| <span data-ttu-id="c3f6b-106">方法</span><span class="sxs-lookup"><span data-stu-id="c3f6b-106">Method</span></span>           | <span data-ttu-id="c3f6b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c3f6b-107">Return Type</span></span>    |<span data-ttu-id="c3f6b-108">说明</span><span class="sxs-lookup"><span data-stu-id="c3f6b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3f6b-109">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="c3f6b-109">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="c3f6b-110">signIn</span><span class="sxs-lookup"><span data-stu-id="c3f6b-110">signIn</span></span>](signin.md) |<span data-ttu-id="c3f6b-111">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-111">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="c3f6b-112">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="c3f6b-112">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="c3f6b-113">signIn</span><span class="sxs-lookup"><span data-stu-id="c3f6b-113">signIn</span></span>](signin.md) |<span data-ttu-id="c3f6b-114">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-114">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3f6b-115">属性</span><span class="sxs-lookup"><span data-stu-id="c3f6b-115">Properties</span></span>
| <span data-ttu-id="c3f6b-116">属性</span><span class="sxs-lookup"><span data-stu-id="c3f6b-116">Property</span></span>     | <span data-ttu-id="c3f6b-117">类型</span><span class="sxs-lookup"><span data-stu-id="c3f6b-117">Type</span></span>   |<span data-ttu-id="c3f6b-118">说明</span><span class="sxs-lookup"><span data-stu-id="c3f6b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3f6b-119">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="c3f6b-119">appDisplayName</span></span>|<span data-ttu-id="c3f6b-120">String</span><span class="sxs-lookup"><span data-stu-id="c3f6b-120">String</span></span>|<span data-ttu-id="c3f6b-121">Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-121">App name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="c3f6b-122">appId</span><span class="sxs-lookup"><span data-stu-id="c3f6b-122">appId</span></span>|<span data-ttu-id="c3f6b-123">String</span><span class="sxs-lookup"><span data-stu-id="c3f6b-123">String</span></span>|<span data-ttu-id="c3f6b-124">表示 Azure Active Directory 中的应用程序 ID 的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-124">Unique GUID representing the app ID in the Azure Active Directory.</span></span>|
|<span data-ttu-id="c3f6b-125">appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="c3f6b-125">appliedConditionalAccessPolicy</span></span>|<span data-ttu-id="c3f6b-126">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="c3f6b-126">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection</span></span>|<span data-ttu-id="c3f6b-127">提供由相应登录活动触发的条件访问策略列表。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-127">Provides a list of conditional access policies that are triggered by the corresponding sign-in activity.</span></span>|
|<span data-ttu-id="c3f6b-128">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="c3f6b-128">clientAppUsed</span></span>|<span data-ttu-id="c3f6b-129">String</span><span class="sxs-lookup"><span data-stu-id="c3f6b-129">String</span></span>|<span data-ttu-id="c3f6b-130">标识用于登录活动的旧客户端。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-130">Identifies the legacy client used for sign-in activity.</span></span>  <span data-ttu-id="c3f6b-131">包括浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI、SMTP 和 POP。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-131">Includes Browser, Exchange Active Sync, modern clients, IMAP, MAPI, SMTP, and POP.</span></span>|
|<span data-ttu-id="c3f6b-132">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="c3f6b-132">conditionalAccessStatus</span></span>|<span data-ttu-id="c3f6b-133">string</span><span class="sxs-lookup"><span data-stu-id="c3f6b-133">string</span></span>| <span data-ttu-id="c3f6b-134">报告激活的条件访问策略的状态。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-134">Reports status of an activated conditional access policy.</span></span> <span data-ttu-id="c3f6b-135">可能的值是`success`: `failure`、 `notApplied`、和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-135">Possible values are: `success`, `failure`, `notApplied`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c3f6b-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="c3f6b-136">correlationId</span></span>|<span data-ttu-id="c3f6b-137">String</span><span class="sxs-lookup"><span data-stu-id="c3f6b-137">String</span></span>|<span data-ttu-id="c3f6b-138">启动登录时从客户端发送的请求 ID;用于对登录活动进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-138">The request ID sent from the client when the sign-in is initiated; used to troubleshoot sign-in activity.</span></span>|
|<span data-ttu-id="c3f6b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3f6b-139">createdDateTime</span></span>|<span data-ttu-id="c3f6b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3f6b-140">DateTimeOffset</span></span>|<span data-ttu-id="c3f6b-141">启动登录的日期和时间 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-141">Date and time (UTC) the sign-in was initiated.</span></span> <span data-ttu-id="c3f6b-142">示例: 2014 年1月1日午夜, 报告`'2014-01-01T00:00:00Z'`为。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-142">Example: midnight on Jan 1, 2014 is reported as `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="c3f6b-143">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="c3f6b-143">deviceDetail</span></span>|[<span data-ttu-id="c3f6b-144">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="c3f6b-144">deviceDetail</span></span>](devicedetail.md)|<span data-ttu-id="c3f6b-145">发生登录的设备信息;包括设备 ID、操作系统和浏览器。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-145">Device information from where the sign-in occurred; includes device ID, operating system, and browser.</span></span> |
|<span data-ttu-id="c3f6b-146">id</span><span class="sxs-lookup"><span data-stu-id="c3f6b-146">id</span></span>|<span data-ttu-id="c3f6b-147">String</span><span class="sxs-lookup"><span data-stu-id="c3f6b-147">String</span></span>|<span data-ttu-id="c3f6b-148">表示登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-148">Unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="c3f6b-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c3f6b-149">ipAddress</span></span>|<span data-ttu-id="c3f6b-150">String</span><span class="sxs-lookup"><span data-stu-id="c3f6b-150">String</span></span>|<span data-ttu-id="c3f6b-151">用于登录的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-151">IP address of the client used to sign in.</span></span>|
|<span data-ttu-id="c3f6b-152">isInteractive</span><span class="sxs-lookup"><span data-stu-id="c3f6b-152">isInteractive</span></span>|<span data-ttu-id="c3f6b-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3f6b-153">Boolean</span></span>|<span data-ttu-id="c3f6b-154">指示登录是否为交互式登录。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-154">Indicates if a sign-in is interactive or not.</span></span>|
|<span data-ttu-id="c3f6b-155">location</span><span class="sxs-lookup"><span data-stu-id="c3f6b-155">location</span></span>|[<span data-ttu-id="c3f6b-156">signInLocation</span><span class="sxs-lookup"><span data-stu-id="c3f6b-156">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="c3f6b-157">提供登录所源于的城市、州和国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-157">Provides the city, state, and country code where the sign-in originated.</span></span>|
|<span data-ttu-id="c3f6b-158">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c3f6b-158">resourceDisplayName</span></span>|<span data-ttu-id="c3f6b-159">字符串</span><span class="sxs-lookup"><span data-stu-id="c3f6b-159">String</span></span>|<span data-ttu-id="c3f6b-160">用户登录到的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-160">Name of the resource the user signed into.</span></span>|
|<span data-ttu-id="c3f6b-161">resourceId</span><span class="sxs-lookup"><span data-stu-id="c3f6b-161">resourceId</span></span>|<span data-ttu-id="c3f6b-162">String</span><span class="sxs-lookup"><span data-stu-id="c3f6b-162">String</span></span>|<span data-ttu-id="c3f6b-163">用户登录到的资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-163">ID of the resource that the user signed into.</span></span>|
|<span data-ttu-id="c3f6b-164">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c3f6b-164">riskDetail</span></span>|<span data-ttu-id="c3f6b-165">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c3f6b-165">riskDetail</span></span>|<span data-ttu-id="c3f6b-166">提供风险用户、登录或风险事件的特定状态背后的“原因”。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-166">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="c3f6b-167">可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-167">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="c3f6b-168">值 `none` 表示到目前为止尚未对用户或登录执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-168">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> <br><span data-ttu-id="c3f6b-169">**注意:** 此属性的详细信息需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-169">**Note:** Details for this property require an Azure AD Premium P2 license.</span></span> <span data-ttu-id="c3f6b-170">其他许可证返回值`hidden`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-170">Other licenses return the value `hidden`.</span></span>|
|<span data-ttu-id="c3f6b-171">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="c3f6b-171">riskEventTypes</span></span>|<span data-ttu-id="c3f6b-172">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="c3f6b-172">riskEventTypes</span></span>|<span data-ttu-id="c3f6b-173">与登录相关联的风险事件类型。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-173">Risk event types associated with the sign-in.</span></span> <span data-ttu-id="c3f6b-174">可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-174">The possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c3f6b-175">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="c3f6b-175">riskLevelAggregated</span></span>|<span data-ttu-id="c3f6b-176">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c3f6b-176">riskLevel</span></span>|<span data-ttu-id="c3f6b-177">聚合风险级别。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-177">Aggregated risk level.</span></span> <span data-ttu-id="c3f6b-178">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-178">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="c3f6b-179">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-179">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="c3f6b-180">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-180">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="c3f6b-181">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-181">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="c3f6b-182">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="c3f6b-182">riskLevelDuringSignIn</span></span>|<span data-ttu-id="c3f6b-183">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c3f6b-183">riskLevel</span></span>|<span data-ttu-id="c3f6b-184">登录过程中的风险级别。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-184">Risk level during sign-in.</span></span> <span data-ttu-id="c3f6b-185">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-185">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="c3f6b-186">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-186">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="c3f6b-187">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-187">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="c3f6b-188">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-188">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="c3f6b-189">riskState</span><span class="sxs-lookup"><span data-stu-id="c3f6b-189">riskState</span></span>|<span data-ttu-id="c3f6b-190">riskState</span><span class="sxs-lookup"><span data-stu-id="c3f6b-190">riskState</span></span>|<span data-ttu-id="c3f6b-191">报告有风险的用户、登录或风险事件的状态。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-191">Reports status of the risky user, sign-in, or a risk event.</span></span> <span data-ttu-id="c3f6b-192">可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-192">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c3f6b-193">status</span><span class="sxs-lookup"><span data-stu-id="c3f6b-193">status</span></span>|[<span data-ttu-id="c3f6b-194">signInStatus</span><span class="sxs-lookup"><span data-stu-id="c3f6b-194">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="c3f6b-195">登录状态。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-195">Sign-in status.</span></span> <span data-ttu-id="c3f6b-196">可取值包括 `Success` 和 `Failure`。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-196">Possible values include `Success` and `Failure`.</span></span>|
|<span data-ttu-id="c3f6b-197">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c3f6b-197">userDisplayName</span></span>|<span data-ttu-id="c3f6b-198">字符串</span><span class="sxs-lookup"><span data-stu-id="c3f6b-198">String</span></span>|<span data-ttu-id="c3f6b-199">启动登录的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-199">Display name of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="c3f6b-200">userId</span><span class="sxs-lookup"><span data-stu-id="c3f6b-200">userId</span></span>|<span data-ttu-id="c3f6b-201">字符串</span><span class="sxs-lookup"><span data-stu-id="c3f6b-201">String</span></span>|<span data-ttu-id="c3f6b-202">启动登录的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-202">ID of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="c3f6b-203">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c3f6b-203">userPrincipalName</span></span>|<span data-ttu-id="c3f6b-204">字符串</span><span class="sxs-lookup"><span data-stu-id="c3f6b-204">String</span></span>|<span data-ttu-id="c3f6b-205">启动登录的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-205">User principal name of the user that initiated the sign-in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3f6b-206">关系</span><span class="sxs-lookup"><span data-stu-id="c3f6b-206">Relationships</span></span>

<span data-ttu-id="c3f6b-207">无</span><span class="sxs-lookup"><span data-stu-id="c3f6b-207">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c3f6b-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3f6b-208">JSON representation</span></span>

<span data-ttu-id="c3f6b-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3f6b-209">Here is a JSON representation of the resource.</span></span>

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
  "riskEventTypes": "string",
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
