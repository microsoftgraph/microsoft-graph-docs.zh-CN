---
title: riskDetection 资源类型
description: 表示 AzureAD 租户中的所有风险检测。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: af77e46c688d514f3a7b49aff3c785712706f3e2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960346"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="5e7a4-103">riskDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e7a4-103">riskDetection resource type</span></span>

<span data-ttu-id="5e7a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e7a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e7a4-105">表示有关 Azure AD 租户中检测到的风险的信息。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-105">Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="5e7a4-106">Azure AD 根据[](riskyuser.md)各种信号和机器学习持续评估[](signin.md)用户风险以及应用或用户登录风险。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-106">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="5e7a4-107">此 API 提供对 Azure AD 环境中的所有风险检测的编程访问权限。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-107">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="5e7a4-108">有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="5e7a4-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

>[!NOTE]
><span data-ttu-id="5e7a4-109">必须具有 Azure AD Premium P1 或 P2 许可证才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-109">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="5e7a4-110">Methods</span><span class="sxs-lookup"><span data-stu-id="5e7a4-110">Methods</span></span>

| <span data-ttu-id="5e7a4-111">方法</span><span class="sxs-lookup"><span data-stu-id="5e7a4-111">Method</span></span>   | <span data-ttu-id="5e7a4-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e7a4-112">Return Type</span></span>|<span data-ttu-id="5e7a4-113">说明</span><span class="sxs-lookup"><span data-stu-id="5e7a4-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e7a4-114">列出 riskDetection</span><span class="sxs-lookup"><span data-stu-id="5e7a4-114">List riskDetection</span></span>](../api/riskdetection-list.md) | <span data-ttu-id="5e7a4-115">[riskDetection](riskdetection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e7a4-115">[riskDetection](riskdetection.md) collection</span></span>|<span data-ttu-id="5e7a4-116">列出风险检测及其属性。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-116">List risk detections and their properties.</span></span>|
|[<span data-ttu-id="5e7a4-117">获取 riskDetection</span><span class="sxs-lookup"><span data-stu-id="5e7a4-117">Get riskDetection</span></span>](../api/riskdetection-get.md) | [<span data-ttu-id="5e7a4-118">riskDetection</span><span class="sxs-lookup"><span data-stu-id="5e7a4-118">riskDetection</span></span>](riskdetection.md)|<span data-ttu-id="5e7a4-119">获取特定的风险检测及其属性。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-119">Get a specific risky detection and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e7a4-120">属性</span><span class="sxs-lookup"><span data-stu-id="5e7a4-120">Properties</span></span>

| <span data-ttu-id="5e7a4-121">属性</span><span class="sxs-lookup"><span data-stu-id="5e7a4-121">Property</span></span>   | <span data-ttu-id="5e7a4-122">类型</span><span class="sxs-lookup"><span data-stu-id="5e7a4-122">Type</span></span>|<span data-ttu-id="5e7a4-123">说明</span><span class="sxs-lookup"><span data-stu-id="5e7a4-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e7a4-124">id</span><span class="sxs-lookup"><span data-stu-id="5e7a4-124">id</span></span>|<span data-ttu-id="5e7a4-125">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-125">string</span></span>|<span data-ttu-id="5e7a4-126">风险检测的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-126">Unique ID of the risk detection.</span></span> |
|<span data-ttu-id="5e7a4-127">requestId</span><span class="sxs-lookup"><span data-stu-id="5e7a4-127">requestId</span></span>|<span data-ttu-id="5e7a4-128">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-128">string</span></span>|<span data-ttu-id="5e7a4-129">与风险检测相关联的登录请求 ID。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-129">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="5e7a4-130">如果风险检测未与登录相关联，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-130">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|<span data-ttu-id="5e7a4-131">correlationId</span><span class="sxs-lookup"><span data-stu-id="5e7a4-131">correlationId</span></span>|<span data-ttu-id="5e7a4-132">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-132">string</span></span>|<span data-ttu-id="5e7a4-133">与风险检测关联的登录的相关 ID。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-133">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="5e7a4-134">如果风险检测未与登录相关联，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-134">This property is null if the risk detection is not associated with a sign-in.</span></span> |
|<span data-ttu-id="5e7a4-135">riskEventType</span><span class="sxs-lookup"><span data-stu-id="5e7a4-135">riskEventType</span></span>|<span data-ttu-id="5e7a4-136">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-136">string</span></span>|<span data-ttu-id="5e7a4-137">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-137">The type of risk event detected.</span></span> <span data-ttu-id="5e7a4-138">可能的值为 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` 、、、、、、、、 `leakedCredentials` `investigationsThreatIntelligence` 和 `generic` `adminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-138">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`,`adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
|<span data-ttu-id="5e7a4-139">riskType</span><span class="sxs-lookup"><span data-stu-id="5e7a4-139">riskType</span></span>|<span data-ttu-id="5e7a4-140">riskEventType</span><span class="sxs-lookup"><span data-stu-id="5e7a4-140">riskEventType</span></span>|<span data-ttu-id="5e7a4-141">风险事件类型列表。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-141">List of risk event types.</span></span><br /><span data-ttu-id="5e7a4-142">**注意：** 此属性已弃用。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-142">**Note:** This property is deprecated.</span></span> <span data-ttu-id="5e7a4-143">请 **改为使用 riskEventType。**</span><span class="sxs-lookup"><span data-stu-id="5e7a4-143">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="5e7a4-144">riskState</span><span class="sxs-lookup"><span data-stu-id="5e7a4-144">riskState</span></span>|<span data-ttu-id="5e7a4-145">riskState</span><span class="sxs-lookup"><span data-stu-id="5e7a4-145">riskState</span></span>|<span data-ttu-id="5e7a4-146">检测到有风险的用户或登录的状态。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-146">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="5e7a4-147">可能的值为 `none` `confirmedSafe` `remediated` `dismissed` `atRisk` 、、、 和 `confirmedCompromised` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-147">The possible values are `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, and `unknownFutureValue`.</span></span> |
|<span data-ttu-id="5e7a4-148">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5e7a4-148">riskLevel</span></span>|<span data-ttu-id="5e7a4-149">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5e7a4-149">riskLevel</span></span>|<span data-ttu-id="5e7a4-150">检测到的风险级别。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-150">Level of the detected risk.</span></span> <span data-ttu-id="5e7a4-151">可能的值为 `low` `medium` `high` `hidden` `none` `unknownFutureValue` 、、、。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-151">The possible values are `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <br /><span data-ttu-id="5e7a4-152">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-152">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="5e7a4-153">将返回 P1 客户 `hidden` 。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-153">P1 customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="5e7a4-154">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5e7a4-154">riskDetail</span></span>|<span data-ttu-id="5e7a4-155">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5e7a4-155">riskDetail</span></span>|<span data-ttu-id="5e7a4-156">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-156">Details of the detected risk.</span></span> <span data-ttu-id="5e7a4-157">可能的值为 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` 、、、、、、、、、 `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-157">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span> <br /><span data-ttu-id="5e7a4-158">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-158">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="5e7a4-159">将返回 P1 客户 `hidden` 。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-159">P1 customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="5e7a4-160">source</span><span class="sxs-lookup"><span data-stu-id="5e7a4-160">source</span></span>|<span data-ttu-id="5e7a4-161">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-161">string</span></span>|<span data-ttu-id="5e7a4-162">风险检测的来源。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-162">Source of the risk detection.</span></span> <span data-ttu-id="5e7a4-163">例如，`activeDirectory`。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-163">For example, `activeDirectory`.</span></span> |
|<span data-ttu-id="5e7a4-164">detectionTimingType</span><span class="sxs-lookup"><span data-stu-id="5e7a4-164">detectionTimingType</span></span>|<span data-ttu-id="5e7a4-165">riskDetectionTimingType</span><span class="sxs-lookup"><span data-stu-id="5e7a4-165">riskDetectionTimingType</span></span>|<span data-ttu-id="5e7a4-166">实时/脱机 (检测到的风险) 。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-166">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="5e7a4-167">可能的值为 `notDefined` `realtime` `nearRealtime` `offline` `unknownFutureValue` 、、。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-167">The possible values are `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.</span></span> |
|<span data-ttu-id="5e7a4-168">活动</span><span class="sxs-lookup"><span data-stu-id="5e7a4-168">activity</span></span>|<span data-ttu-id="5e7a4-169">activityType</span><span class="sxs-lookup"><span data-stu-id="5e7a4-169">activityType</span></span>|<span data-ttu-id="5e7a4-170">指示检测到的风险链接到的活动类型。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-170">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="5e7a4-171">可能的值为 `signin` `user` `unknownFutureValue` 、、。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-171">The possible values are `signin`, `user`, `unknownFutureValue`.</span></span> |
|<span data-ttu-id="5e7a4-172">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="5e7a4-172">tokenIssuerType</span></span>|<span data-ttu-id="5e7a4-173">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="5e7a4-173">tokenIssuerType</span></span>|<span data-ttu-id="5e7a4-174">指示检测到的登录风险的令牌颁发者类型。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-174">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="5e7a4-175">可取值为：`AzureAD`、`ADFederationServices` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-175">The possible values are `AzureAD`, `ADFederationServices`, and `unknownFutureValue`.</span></span> |
|<span data-ttu-id="5e7a4-176">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5e7a4-176">ipAddress</span></span>|<span data-ttu-id="5e7a4-177">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-177">string</span></span>|<span data-ttu-id="5e7a4-178">提供发生风险的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-178">Provides the IP address of the client from where the risk occurred.</span></span> |
|<span data-ttu-id="5e7a4-179">location</span><span class="sxs-lookup"><span data-stu-id="5e7a4-179">location</span></span>|[<span data-ttu-id="5e7a4-180">signInLocation</span><span class="sxs-lookup"><span data-stu-id="5e7a4-180">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="5e7a4-181">登录的位置。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-181">Location of the sign-in.</span></span> |
|<span data-ttu-id="5e7a4-182">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="5e7a4-182">activityDateTime</span></span>|<span data-ttu-id="5e7a4-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7a4-183">DateTimeOffset</span></span>|<span data-ttu-id="5e7a4-184">发生有风险活动的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-184">Date and time that the risky activity occurred.</span></span> <span data-ttu-id="5e7a4-185">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-185">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e7a4-186">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5e7a4-186">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5e7a4-187">detectedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e7a4-187">detectedDateTime</span></span>|<span data-ttu-id="5e7a4-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7a4-188">DateTimeOffset</span></span>|<span data-ttu-id="5e7a4-189">检测到风险的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-189">Date and time that the risk was detected.</span></span> <span data-ttu-id="5e7a4-190">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-190">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e7a4-191">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5e7a4-191">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
|<span data-ttu-id="5e7a4-192">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e7a4-192">lastUpdatedDateTime</span></span>|<span data-ttu-id="5e7a4-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7a4-193">DateTimeOffset</span></span>|<span data-ttu-id="5e7a4-194">上次更新风险检测的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-194">Date and time that the risk detection was last updated.</span></span> |
|<span data-ttu-id="5e7a4-195">userId</span><span class="sxs-lookup"><span data-stu-id="5e7a4-195">userId</span></span>|<span data-ttu-id="5e7a4-196">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-196">string</span></span>|<span data-ttu-id="5e7a4-197">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-197">Unique ID of the user.</span></span>  <span data-ttu-id="5e7a4-198">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-198">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e7a4-199">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5e7a4-199">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5e7a4-200">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5e7a4-200">userDisplayName</span></span>|<span data-ttu-id="5e7a4-201">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-201">string</span></span>|<span data-ttu-id="5e7a4-202">用户名。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-202">Name of the user.</span></span> |
|<span data-ttu-id="5e7a4-203">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e7a4-203">userPrincipalName</span></span>|<span data-ttu-id="5e7a4-204">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-204">string</span></span>|<span data-ttu-id="5e7a4-205">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-205">The user principal name (UPN) of the user.</span></span> |
|<span data-ttu-id="5e7a4-206">additionalInfo</span><span class="sxs-lookup"><span data-stu-id="5e7a4-206">additionalInfo</span></span>|<span data-ttu-id="5e7a4-207">string</span><span class="sxs-lookup"><span data-stu-id="5e7a4-207">string</span></span>|<span data-ttu-id="5e7a4-208">与 JSON 格式的风险检测相关的其他信息。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-208">Additional information associated with the risk detection in JSON format.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5e7a4-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e7a4-209">JSON representation</span></span>

<span data-ttu-id="5e7a4-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e7a4-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
