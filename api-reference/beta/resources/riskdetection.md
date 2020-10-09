---
title: riskDetection 资源类型
description: 表示 AzureAD 租户中的所有风险检测。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ac9606b0b1d2a5bd49ac25f25ce43996b9bb60a1
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400730"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="71d2a-103">riskDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="71d2a-103">riskDetection resource type</span></span>

<span data-ttu-id="71d2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71d2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71d2a-105">表示有关 Azure AD 租户中检测到的风险的信息。</span><span class="sxs-lookup"><span data-stu-id="71d2a-105">Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="71d2a-106">Azure AD 会根据各种信号和机器学习持续评估 [用户风险](riskyuser.md) 和应用或用户 [登录](signin.md) 风险。</span><span class="sxs-lookup"><span data-stu-id="71d2a-106">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="71d2a-107">此 API 提供对 Azure AD 环境中所有风险检测的编程访问。</span><span class="sxs-lookup"><span data-stu-id="71d2a-107">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="71d2a-108">有关风险事件的详细信息，请参阅 [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="71d2a-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

>[!NOTE]
><span data-ttu-id="71d2a-109">您必须具有 Azure AD 高级 P1 或 P2 许可证，才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="71d2a-109">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="71d2a-110">方法</span><span class="sxs-lookup"><span data-stu-id="71d2a-110">Methods</span></span>

| <span data-ttu-id="71d2a-111">方法</span><span class="sxs-lookup"><span data-stu-id="71d2a-111">Method</span></span>   | <span data-ttu-id="71d2a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="71d2a-112">Return Type</span></span>|<span data-ttu-id="71d2a-113">说明</span><span class="sxs-lookup"><span data-stu-id="71d2a-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71d2a-114">列出 riskDetection</span><span class="sxs-lookup"><span data-stu-id="71d2a-114">List riskDetection</span></span>](../api/riskdetection-list.md) | <span data-ttu-id="71d2a-115">[riskDetection](riskdetection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71d2a-115">[riskDetection](riskdetection.md) collection</span></span>|<span data-ttu-id="71d2a-116">列出风险检测及其属性。</span><span class="sxs-lookup"><span data-stu-id="71d2a-116">List risk detections and their properties.</span></span>|
|[<span data-ttu-id="71d2a-117">获取 riskDetection</span><span class="sxs-lookup"><span data-stu-id="71d2a-117">Get riskDetection</span></span>](../api/riskdetection-get.md) | [<span data-ttu-id="71d2a-118">riskDetection</span><span class="sxs-lookup"><span data-stu-id="71d2a-118">riskDetection</span></span>](riskdetection.md)|<span data-ttu-id="71d2a-119">获取特定的风险检测及其属性。</span><span class="sxs-lookup"><span data-stu-id="71d2a-119">Get a specific risky detection and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="71d2a-120">属性</span><span class="sxs-lookup"><span data-stu-id="71d2a-120">Properties</span></span>

| <span data-ttu-id="71d2a-121">属性</span><span class="sxs-lookup"><span data-stu-id="71d2a-121">Property</span></span>   | <span data-ttu-id="71d2a-122">类型</span><span class="sxs-lookup"><span data-stu-id="71d2a-122">Type</span></span>|<span data-ttu-id="71d2a-123">说明</span><span class="sxs-lookup"><span data-stu-id="71d2a-123">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="71d2a-124">风险检测的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="71d2a-124">Unique ID of the risk detection.</span></span> |
|`requestId`|`string`|<span data-ttu-id="71d2a-125">与风险检测相关联的登录请求 ID。</span><span class="sxs-lookup"><span data-stu-id="71d2a-125">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="71d2a-126">如果风险检测未与登录相关联，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="71d2a-126">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|`correlationId`|`string`|<span data-ttu-id="71d2a-127">与风险检测相关联的登录的相关 ID。</span><span class="sxs-lookup"><span data-stu-id="71d2a-127">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="71d2a-128">如果风险检测未与登录相关联，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="71d2a-128">This property is null if the risk detection is not associated with a sign-in.</span></span> |
|`riskEventType`|`string`|<span data-ttu-id="71d2a-129">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="71d2a-129">The type of risk event detected.</span></span> <span data-ttu-id="71d2a-130">可能的值为、、、、、、、、、、、、 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` 和 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="71d2a-130">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
|`riskType`|`riskEventType`|<span data-ttu-id="71d2a-131">风险事件类型的列表。</span><span class="sxs-lookup"><span data-stu-id="71d2a-131">List of risk event types.</span></span><br/><span data-ttu-id="71d2a-132">**注意：** 此属性已被弃用。</span><span class="sxs-lookup"><span data-stu-id="71d2a-132">**Note:** This property is deprecated.</span></span> <span data-ttu-id="71d2a-133">请改用 **riskEventTypes** 。</span><span class="sxs-lookup"><span data-stu-id="71d2a-133">Use **riskEventTypes** instead.</span></span> |
|`riskState`|`riskState`|<span data-ttu-id="71d2a-134">检测到的有风险的用户或登录的状态。</span><span class="sxs-lookup"><span data-stu-id="71d2a-134">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="71d2a-135">可能的值为 none、confirmedSafe、已修正、已消除、atRisk、confirmedCompromised 和向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="71d2a-135">The possible values are none, confirmedSafe, remediated, dismissed, atRisk, confirmedCompromised, and unknownFutureValue.</span></span> |
|`riskLevel`|`riskLevel`|<span data-ttu-id="71d2a-136">检测到的风险的级别。</span><span class="sxs-lookup"><span data-stu-id="71d2a-136">Level of the detected risk.</span></span> <span data-ttu-id="71d2a-137">可能的值为 low、medium、high、hidden、none、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="71d2a-137">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span> <span data-ttu-id="71d2a-138">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="71d2a-138">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="71d2a-139">将返回 P1 客户 `hidden` 。</span><span class="sxs-lookup"><span data-stu-id="71d2a-139">P1 customers will be returned `hidden`.</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="71d2a-140">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="71d2a-140">Details of the detected risk.</span></span> <span data-ttu-id="71d2a-141">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="71d2a-141">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span> <span data-ttu-id="71d2a-142">**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。</span><span class="sxs-lookup"><span data-stu-id="71d2a-142">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="71d2a-143">将返回 P1 客户 `hidden` 。</span><span class="sxs-lookup"><span data-stu-id="71d2a-143">P1 customers will be returned `hidden`.</span></span>|
|`source`|`string`|<span data-ttu-id="71d2a-144">风险检测的来源。</span><span class="sxs-lookup"><span data-stu-id="71d2a-144">Source of the risk detection.</span></span> <span data-ttu-id="71d2a-145">例如，"activeDirectory"。</span><span class="sxs-lookup"><span data-stu-id="71d2a-145">For example, "activeDirectory".</span></span> |
|`detectionTimingType`|`riskDetectionTimingType`|<span data-ttu-id="71d2a-146">检测到的风险 (实时/脱机) 的时间。</span><span class="sxs-lookup"><span data-stu-id="71d2a-146">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="71d2a-147">可能的值包括 notDefined、实时、nearRealtime、offline 和向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="71d2a-147">The possible values are notDefined, realtime, nearRealtime, offline, unknownFutureValue.</span></span> |
|`activity`|`activityType`|<span data-ttu-id="71d2a-148">指示检测到的风险所链接到的活动类型。</span><span class="sxs-lookup"><span data-stu-id="71d2a-148">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="71d2a-149">可能的值为 "登录"、"用户"、"向 unknownfuturevalue"。</span><span class="sxs-lookup"><span data-stu-id="71d2a-149">The possible values are signin, user, unknownFutureValue.</span></span> |
|`tokenIssuerType`|`tokenIssuerType`|<span data-ttu-id="71d2a-150">指示检测到的登录风险的令牌颁发者的类型。</span><span class="sxs-lookup"><span data-stu-id="71d2a-150">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="71d2a-151">可能的值是 AzureAD、ADFederationServices 和向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="71d2a-151">The possible values are AzureAD, ADFederationServices, and unknownFutureValue.</span></span> |
|`ipAddress`|`string`|<span data-ttu-id="71d2a-152">提供从其发生风险的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="71d2a-152">Provides the IP address of the client from where the risk occurred.</span></span> |
|`location`|[<span data-ttu-id="71d2a-153">signInLocation</span><span class="sxs-lookup"><span data-stu-id="71d2a-153">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="71d2a-154">登录的位置。</span><span class="sxs-lookup"><span data-stu-id="71d2a-154">Location of the sign-in.</span></span> |
|`activityDateTime`|`datetimeoffset`|<span data-ttu-id="71d2a-155">风险活动发生的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="71d2a-155">Date and time that the risky activity occurred.</span></span> |
|`detectedDateTime`|`datetimeoffset`|<span data-ttu-id="71d2a-156">检测到风险的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="71d2a-156">Date and time that the risk was detected.</span></span> |
|`lastUpdatedDateTime`|`datetime`|<span data-ttu-id="71d2a-157">上次更新风险检测的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="71d2a-157">Date and time that the risk detection was last updated.</span></span> |
|`userId`|`string`|<span data-ttu-id="71d2a-158">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="71d2a-158">Unique ID of the user.</span></span> |
|`userDisplayName`|`string`|<span data-ttu-id="71d2a-159">用户名。</span><span class="sxs-lookup"><span data-stu-id="71d2a-159">Name of the user.</span></span> |
|`userPrincipalName`|`string`|<span data-ttu-id="71d2a-160">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="71d2a-160">The user principal name (UPN) of the user.</span></span> |
|`additionalInfo`|`string`|<span data-ttu-id="71d2a-161">与以 JSON 格式进行的风险检测相关联的其他信息。</span><span class="sxs-lookup"><span data-stu-id="71d2a-161">Additional information associated with the risk detection in JSON format.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71d2a-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71d2a-162">JSON representation</span></span>

<span data-ttu-id="71d2a-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71d2a-163">The following is a JSON representation of the resource.</span></span>

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