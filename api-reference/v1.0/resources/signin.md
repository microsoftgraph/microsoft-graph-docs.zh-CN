---
title: signIn 资源类型
description: 详细介绍租户（目录）的用户和应用程序登录活动。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 367be35ffc1c37b04f2c3f5f1c70139e4562c870
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533716"
---
# <a name="signin-resource-type"></a><span data-ttu-id="8f8f3-103">signIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f8f3-103">signIn resource type</span></span>

<span data-ttu-id="8f8f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f8f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f8f3-105">详细介绍租户（目录）的用户和应用程序登录活动。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-105">Details user and application sign-in activity for a tenant (directory).</span></span>

## <a name="methods"></a><span data-ttu-id="8f8f3-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8f8f3-106">Methods</span></span>

| <span data-ttu-id="8f8f3-107">方法</span><span class="sxs-lookup"><span data-stu-id="8f8f3-107">Method</span></span>           | <span data-ttu-id="8f8f3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f8f3-108">Return Type</span></span>    |<span data-ttu-id="8f8f3-109">说明</span><span class="sxs-lookup"><span data-stu-id="8f8f3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f8f3-110">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="8f8f3-110">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="8f8f3-111">signIn</span><span class="sxs-lookup"><span data-stu-id="8f8f3-111">signIn</span></span>](signin.md) |<span data-ttu-id="8f8f3-112">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-112">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="8f8f3-113">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="8f8f3-113">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="8f8f3-114">signIn</span><span class="sxs-lookup"><span data-stu-id="8f8f3-114">signIn</span></span>](signin.md) |<span data-ttu-id="8f8f3-115">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-115">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f8f3-116">属性</span><span class="sxs-lookup"><span data-stu-id="8f8f3-116">Properties</span></span>
| <span data-ttu-id="8f8f3-117">属性</span><span class="sxs-lookup"><span data-stu-id="8f8f3-117">Property</span></span>     | <span data-ttu-id="8f8f3-118">类型</span><span class="sxs-lookup"><span data-stu-id="8f8f3-118">Type</span></span>   |<span data-ttu-id="8f8f3-119">说明</span><span class="sxs-lookup"><span data-stu-id="8f8f3-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f8f3-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="8f8f3-120">appDisplayName</span></span>|<span data-ttu-id="8f8f3-121">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-121">String</span></span>|<span data-ttu-id="8f8f3-122">Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-122">App name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="8f8f3-123">appId</span><span class="sxs-lookup"><span data-stu-id="8f8f3-123">appId</span></span>|<span data-ttu-id="8f8f3-124">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-124">String</span></span>|<span data-ttu-id="8f8f3-125">表示 Azure Active Directory 中的应用程序 ID 的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-125">Unique GUID representing the app ID in the Azure Active Directory.</span></span>|
|<span data-ttu-id="8f8f3-126">appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="8f8f3-126">appliedConditionalAccessPolicy</span></span>|<span data-ttu-id="8f8f3-127">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="8f8f3-127">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection</span></span>|<span data-ttu-id="8f8f3-128">提供由相应登录活动触发的条件访问策略列表。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-128">Provides a list of conditional access policies that are triggered by the corresponding sign-in activity.</span></span>|
|<span data-ttu-id="8f8f3-129">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="8f8f3-129">clientAppUsed</span></span>|<span data-ttu-id="8f8f3-130">String</span><span class="sxs-lookup"><span data-stu-id="8f8f3-130">String</span></span>|<span data-ttu-id="8f8f3-131">标识用于登录活动的旧客户端。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-131">Identifies the legacy client used for sign-in activity.</span></span>  <span data-ttu-id="8f8f3-132">包括浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI、SMTP 和 POP。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-132">Includes Browser, Exchange Active Sync, modern clients, IMAP, MAPI, SMTP, and POP.</span></span>|
|<span data-ttu-id="8f8f3-133">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="8f8f3-133">conditionalAccessStatus</span></span>|<span data-ttu-id="8f8f3-134">string</span><span class="sxs-lookup"><span data-stu-id="8f8f3-134">string</span></span>| <span data-ttu-id="8f8f3-135">报告激活的条件访问策略的状态。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-135">Reports status of an activated conditional access policy.</span></span> <span data-ttu-id="8f8f3-136">可能的值是`success`： `failure`、 `notApplied`、和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-136">Possible values are: `success`, `failure`, `notApplied`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8f8f3-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="8f8f3-137">correlationId</span></span>|<span data-ttu-id="8f8f3-138">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-138">String</span></span>|<span data-ttu-id="8f8f3-139">启动登录时从客户端发送的请求 ID;用于对登录活动进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-139">The request ID sent from the client when the sign-in is initiated; used to troubleshoot sign-in activity.</span></span>|
|<span data-ttu-id="8f8f3-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f8f3-140">createdDateTime</span></span>|<span data-ttu-id="8f8f3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f8f3-141">DateTimeOffset</span></span>|<span data-ttu-id="8f8f3-142">启动登录的日期和时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-142">Date and time (UTC) the sign-in was initiated.</span></span> <span data-ttu-id="8f8f3-143">示例：2014年1月1日午夜，报告`'2014-01-01T00:00:00Z'`为。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-143">Example: midnight on Jan 1, 2014 is reported as `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8f8f3-144">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="8f8f3-144">deviceDetail</span></span>|[<span data-ttu-id="8f8f3-145">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="8f8f3-145">deviceDetail</span></span>](devicedetail.md)|<span data-ttu-id="8f8f3-146">发生登录的设备信息;包括设备 ID、操作系统和浏览器。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-146">Device information from where the sign-in occurred; includes device ID, operating system, and browser.</span></span> |
|<span data-ttu-id="8f8f3-147">id</span><span class="sxs-lookup"><span data-stu-id="8f8f3-147">id</span></span>|<span data-ttu-id="8f8f3-148">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-148">String</span></span>|<span data-ttu-id="8f8f3-149">表示登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-149">Unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="8f8f3-150">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8f8f3-150">ipAddress</span></span>|<span data-ttu-id="8f8f3-151">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-151">String</span></span>|<span data-ttu-id="8f8f3-152">用于登录的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-152">IP address of the client used to sign in.</span></span>|
|<span data-ttu-id="8f8f3-153">isInteractive</span><span class="sxs-lookup"><span data-stu-id="8f8f3-153">isInteractive</span></span>|<span data-ttu-id="8f8f3-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f8f3-154">Boolean</span></span>|<span data-ttu-id="8f8f3-155">指示登录是否为交互式登录。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-155">Indicates if a sign-in is interactive or not.</span></span>|
|<span data-ttu-id="8f8f3-156">location</span><span class="sxs-lookup"><span data-stu-id="8f8f3-156">location</span></span>|[<span data-ttu-id="8f8f3-157">signInLocation</span><span class="sxs-lookup"><span data-stu-id="8f8f3-157">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="8f8f3-158">提供登录所源于的城市、州和国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-158">Provides the city, state, and country code where the sign-in originated.</span></span>|
|<span data-ttu-id="8f8f3-159">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8f8f3-159">resourceDisplayName</span></span>|<span data-ttu-id="8f8f3-160">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-160">String</span></span>|<span data-ttu-id="8f8f3-161">用户登录到的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-161">Name of the resource the user signed into.</span></span>|
|<span data-ttu-id="8f8f3-162">resourceId</span><span class="sxs-lookup"><span data-stu-id="8f8f3-162">resourceId</span></span>|<span data-ttu-id="8f8f3-163">String</span><span class="sxs-lookup"><span data-stu-id="8f8f3-163">String</span></span>|<span data-ttu-id="8f8f3-164">用户登录到的资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-164">ID of the resource that the user signed into.</span></span>|
|<span data-ttu-id="8f8f3-165">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8f8f3-165">riskDetail</span></span>|<span data-ttu-id="8f8f3-166">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8f8f3-166">riskDetail</span></span>|<span data-ttu-id="8f8f3-167">提供风险用户、登录或风险事件的特定状态背后的“原因”。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-167">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="8f8f3-168">可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-168">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="8f8f3-169">值 `none` 表示到目前为止尚未对用户或登录执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-169">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> <br><span data-ttu-id="8f8f3-170">**注意：** 此属性的详细信息需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-170">**Note:** Details for this property require an Azure AD Premium P2 license.</span></span> <span data-ttu-id="8f8f3-171">其他许可证返回值`hidden`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-171">Other licenses return the value `hidden`.</span></span>|
|<span data-ttu-id="8f8f3-172">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="8f8f3-172">riskEventTypes</span></span>|<span data-ttu-id="8f8f3-173">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="8f8f3-173">riskEventTypes</span></span>|<span data-ttu-id="8f8f3-174">与登录相关联的风险事件类型。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-174">Risk event types associated with the sign-in.</span></span> <span data-ttu-id="8f8f3-175">可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-175">The possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8f8f3-176">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="8f8f3-176">riskLevelAggregated</span></span>|<span data-ttu-id="8f8f3-177">riskLevel</span><span class="sxs-lookup"><span data-stu-id="8f8f3-177">riskLevel</span></span>|<span data-ttu-id="8f8f3-178">聚合风险级别。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-178">Aggregated risk level.</span></span> <span data-ttu-id="8f8f3-179">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-179">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="8f8f3-180">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-180">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="8f8f3-181">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-181">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="8f8f3-182">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-182">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="8f8f3-183">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="8f8f3-183">riskLevelDuringSignIn</span></span>|<span data-ttu-id="8f8f3-184">riskLevel</span><span class="sxs-lookup"><span data-stu-id="8f8f3-184">riskLevel</span></span>|<span data-ttu-id="8f8f3-185">登录过程中的风险级别。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-185">Risk level during sign-in.</span></span> <span data-ttu-id="8f8f3-186">可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-186">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="8f8f3-187">值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-187">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="8f8f3-188">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-188">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="8f8f3-189">对于所有其他客户，将返回 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-189">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="8f8f3-190">riskState</span><span class="sxs-lookup"><span data-stu-id="8f8f3-190">riskState</span></span>|<span data-ttu-id="8f8f3-191">riskState</span><span class="sxs-lookup"><span data-stu-id="8f8f3-191">riskState</span></span>|<span data-ttu-id="8f8f3-192">报告有风险的用户、登录或风险事件的状态。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-192">Reports status of the risky user, sign-in, or a risk event.</span></span> <span data-ttu-id="8f8f3-193">可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-193">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8f8f3-194">status</span><span class="sxs-lookup"><span data-stu-id="8f8f3-194">status</span></span>|[<span data-ttu-id="8f8f3-195">signInStatus</span><span class="sxs-lookup"><span data-stu-id="8f8f3-195">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="8f8f3-196">登录状态。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-196">Sign-in status.</span></span> <span data-ttu-id="8f8f3-197">可取值包括 `Success` 和 `Failure`。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-197">Possible values include `Success` and `Failure`.</span></span>|
|<span data-ttu-id="8f8f3-198">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8f8f3-198">userDisplayName</span></span>|<span data-ttu-id="8f8f3-199">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-199">String</span></span>|<span data-ttu-id="8f8f3-200">启动登录的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-200">Display name of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="8f8f3-201">userId</span><span class="sxs-lookup"><span data-stu-id="8f8f3-201">userId</span></span>|<span data-ttu-id="8f8f3-202">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-202">String</span></span>|<span data-ttu-id="8f8f3-203">启动登录的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-203">ID of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="8f8f3-204">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8f8f3-204">userPrincipalName</span></span>|<span data-ttu-id="8f8f3-205">字符串</span><span class="sxs-lookup"><span data-stu-id="8f8f3-205">String</span></span>|<span data-ttu-id="8f8f3-206">启动登录的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-206">User principal name of the user that initiated the sign-in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f8f3-207">关系</span><span class="sxs-lookup"><span data-stu-id="8f8f3-207">Relationships</span></span>

<span data-ttu-id="8f8f3-208">无</span><span class="sxs-lookup"><span data-stu-id="8f8f3-208">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f8f3-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f8f3-209">JSON representation</span></span>

<span data-ttu-id="8f8f3-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f8f3-210">Here is a JSON representation of the resource.</span></span>

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
