---
title: riskDetection 资源类型
description: 风险检测
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ad9c9a7ec23efdc86470f8ea3ed5245173cd1d1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896873"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="59bc0-103">riskDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="59bc0-103">riskDetection resource type</span></span>

<span data-ttu-id="59bc0-104">命名空间： microsoft. graph 表示有关 Azure AD 租户中检测到的风险的信息。</span><span class="sxs-lookup"><span data-stu-id="59bc0-104">Namespace: microsoft.graph Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="59bc0-105">Azure AD 会根据各种信号和机器学习持续评估[用户风险](riskyuser.md)和应用或用户[登录](signin.md)风险。</span><span class="sxs-lookup"><span data-stu-id="59bc0-105">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="59bc0-106">此 API 提供对 Azure AD 环境中所有风险检测的编程访问。</span><span class="sxs-lookup"><span data-stu-id="59bc0-106">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="59bc0-107">有关风险事件的详细信息，请参阅[Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)。</span><span class="sxs-lookup"><span data-stu-id="59bc0-107">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

>[!NOTE]
><span data-ttu-id="59bc0-108">您必须具有 Azure AD 高级 P1 或 P2 许可证，才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="59bc0-108">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="59bc0-109">方法</span><span class="sxs-lookup"><span data-stu-id="59bc0-109">Methods</span></span>
|<span data-ttu-id="59bc0-110">方法</span><span class="sxs-lookup"><span data-stu-id="59bc0-110">Method</span></span>|<span data-ttu-id="59bc0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="59bc0-111">Return type</span></span>|<span data-ttu-id="59bc0-112">说明</span><span class="sxs-lookup"><span data-stu-id="59bc0-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59bc0-113">列出 riskDetections</span><span class="sxs-lookup"><span data-stu-id="59bc0-113">List riskDetections</span></span>](../api/riskdetection-list.md)|<span data-ttu-id="59bc0-114">[riskDetection](../resources/riskdetection.md)集合</span><span class="sxs-lookup"><span data-stu-id="59bc0-114">[riskDetection](../resources/riskdetection.md) collection</span></span>|<span data-ttu-id="59bc0-115">获取[riskDetection](../resources/riskdetection.md)对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="59bc0-115">Get a list of the [riskDetection](../resources/riskdetection.md) objects and their properties.</span></span>|
|[<span data-ttu-id="59bc0-116">获取 riskDetection</span><span class="sxs-lookup"><span data-stu-id="59bc0-116">Get riskDetection</span></span>](../api/riskdetection-get.md)|[<span data-ttu-id="59bc0-117">riskDetection</span><span class="sxs-lookup"><span data-stu-id="59bc0-117">riskDetection</span></span>](../resources/riskdetection.md)|<span data-ttu-id="59bc0-118">读取[riskDetection](../resources/riskdetection.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59bc0-118">Read the properties and relationships of a [riskDetection](../resources/riskdetection.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="59bc0-119">属性</span><span class="sxs-lookup"><span data-stu-id="59bc0-119">Properties</span></span>
|<span data-ttu-id="59bc0-120">属性</span><span class="sxs-lookup"><span data-stu-id="59bc0-120">Property</span></span>|<span data-ttu-id="59bc0-121">类型</span><span class="sxs-lookup"><span data-stu-id="59bc0-121">Type</span></span>|<span data-ttu-id="59bc0-122">说明</span><span class="sxs-lookup"><span data-stu-id="59bc0-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59bc0-123">activity</span><span class="sxs-lookup"><span data-stu-id="59bc0-123">activity</span></span>|<span data-ttu-id="59bc0-124">activityType</span><span class="sxs-lookup"><span data-stu-id="59bc0-124">activityType</span></span>|<span data-ttu-id="59bc0-125">指示检测到的风险所链接到的活动类型。</span><span class="sxs-lookup"><span data-stu-id="59bc0-125">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="59bc0-126">.</span><span class="sxs-lookup"><span data-stu-id="59bc0-126">.</span></span> <span data-ttu-id="59bc0-127">可取值为：`signin`、`user`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="59bc0-127">Possible values are: `signin`, `user`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="59bc0-128">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="59bc0-128">activityDateTime</span></span>|<span data-ttu-id="59bc0-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59bc0-129">DateTimeOffset</span></span>|<span data-ttu-id="59bc0-130">风险活动发生的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="59bc0-130">Date and time that the risky activity occurred.</span></span>|
|<span data-ttu-id="59bc0-131">additionalInfo</span><span class="sxs-lookup"><span data-stu-id="59bc0-131">additionalInfo</span></span>|<span data-ttu-id="59bc0-132">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-132">String</span></span>|<span data-ttu-id="59bc0-133">与以 JSON 格式进行的风险检测相关联的其他信息。</span><span class="sxs-lookup"><span data-stu-id="59bc0-133">Additional information associated with the risk detection in JSON format.</span></span>|
|<span data-ttu-id="59bc0-134">correlationId</span><span class="sxs-lookup"><span data-stu-id="59bc0-134">correlationId</span></span>|<span data-ttu-id="59bc0-135">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-135">String</span></span>|<span data-ttu-id="59bc0-136">与风险检测相关联的登录的相关 ID。</span><span class="sxs-lookup"><span data-stu-id="59bc0-136">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="59bc0-137">如果风险检测未与登录相关联，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="59bc0-137">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|<span data-ttu-id="59bc0-138">detectedDateTime</span><span class="sxs-lookup"><span data-stu-id="59bc0-138">detectedDateTime</span></span>|<span data-ttu-id="59bc0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59bc0-139">DateTimeOffset</span></span>|<span data-ttu-id="59bc0-140">检测到风险的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="59bc0-140">Date and time that the risk was detected.</span></span>|
|<span data-ttu-id="59bc0-141">detectionTimingType</span><span class="sxs-lookup"><span data-stu-id="59bc0-141">detectionTimingType</span></span>|<span data-ttu-id="59bc0-142">riskDetectionTimingType</span><span class="sxs-lookup"><span data-stu-id="59bc0-142">riskDetectionTimingType</span></span>|<span data-ttu-id="59bc0-143">检测到的风险的时间段（实时/脱机）。</span><span class="sxs-lookup"><span data-stu-id="59bc0-143">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="59bc0-144">可取值为：`notDefined`、`realtime`、`nearRealtime`、`offline`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="59bc0-144">Possible values are: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="59bc0-145">id</span><span class="sxs-lookup"><span data-stu-id="59bc0-145">id</span></span>|<span data-ttu-id="59bc0-146">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-146">String</span></span>|<span data-ttu-id="59bc0-147">风险检测的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="59bc0-147">Unique ID of the risk detection.</span></span> <span data-ttu-id="59bc0-148">继承自[entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="59bc0-148">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="59bc0-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="59bc0-149">ipAddress</span></span>|<span data-ttu-id="59bc0-150">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-150">String</span></span>|<span data-ttu-id="59bc0-151">提供从其发生风险的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="59bc0-151">Provides the IP address of the client from where the risk occurred.</span></span>|
|<span data-ttu-id="59bc0-152">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="59bc0-152">lastUpdatedDateTime</span></span>|<span data-ttu-id="59bc0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59bc0-153">DateTimeOffset</span></span>|<span data-ttu-id="59bc0-154">上次更新风险检测的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="59bc0-154">Date and time that the risk detection was last updated.</span></span>|
|<span data-ttu-id="59bc0-155">location</span><span class="sxs-lookup"><span data-stu-id="59bc0-155">location</span></span>|[<span data-ttu-id="59bc0-156">signInLocation</span><span class="sxs-lookup"><span data-stu-id="59bc0-156">signInLocation</span></span>](../resources/signinlocation.md)|<span data-ttu-id="59bc0-157">登录的位置。</span><span class="sxs-lookup"><span data-stu-id="59bc0-157">Location of the sign-in.</span></span>|
|<span data-ttu-id="59bc0-158">请求</span><span class="sxs-lookup"><span data-stu-id="59bc0-158">requestId</span></span>|<span data-ttu-id="59bc0-159">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-159">String</span></span>|<span data-ttu-id="59bc0-160">与风险检测相关联的登录请求 ID。</span><span class="sxs-lookup"><span data-stu-id="59bc0-160">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="59bc0-161">如果风险检测未与登录相关联，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="59bc0-161">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|<span data-ttu-id="59bc0-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="59bc0-162">riskDetail</span></span>|<span data-ttu-id="59bc0-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="59bc0-163">riskDetail</span></span>|<span data-ttu-id="59bc0-164">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="59bc0-164">Details of the detected risk.</span></span> <span data-ttu-id="59bc0-165">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="59bc0-165">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="59bc0-166">riskEventType</span><span class="sxs-lookup"><span data-stu-id="59bc0-166">riskEventType</span></span>|<span data-ttu-id="59bc0-167">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-167">String</span></span>|<span data-ttu-id="59bc0-168">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="59bc0-168">The type of risk event detected.</span></span> <span data-ttu-id="59bc0-169">可能的值为、、、、、、、、、、、、 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` 和 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="59bc0-169">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="59bc0-170">riskLevel</span><span class="sxs-lookup"><span data-stu-id="59bc0-170">riskLevel</span></span>|<span data-ttu-id="59bc0-171">riskLevel</span><span class="sxs-lookup"><span data-stu-id="59bc0-171">riskLevel</span></span>|<span data-ttu-id="59bc0-172">检测到的风险的级别。</span><span class="sxs-lookup"><span data-stu-id="59bc0-172">Level of the detected risk.</span></span> <span data-ttu-id="59bc0-173">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="59bc0-173">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="59bc0-174">riskState</span><span class="sxs-lookup"><span data-stu-id="59bc0-174">riskState</span></span>|<span data-ttu-id="59bc0-175">riskState</span><span class="sxs-lookup"><span data-stu-id="59bc0-175">riskState</span></span>|<span data-ttu-id="59bc0-176">检测到的有风险的用户或登录的状态。</span><span class="sxs-lookup"><span data-stu-id="59bc0-176">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="59bc0-177">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="59bc0-177">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="59bc0-178">source</span><span class="sxs-lookup"><span data-stu-id="59bc0-178">source</span></span>|<span data-ttu-id="59bc0-179">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-179">String</span></span>|<span data-ttu-id="59bc0-180">风险检测的来源。</span><span class="sxs-lookup"><span data-stu-id="59bc0-180">Source of the risk detection.</span></span> <span data-ttu-id="59bc0-181">例如，"activeDirectory"。</span><span class="sxs-lookup"><span data-stu-id="59bc0-181">For example, "activeDirectory".</span></span> |
|<span data-ttu-id="59bc0-182">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="59bc0-182">tokenIssuerType</span></span>|<span data-ttu-id="59bc0-183">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="59bc0-183">tokenIssuerType</span></span>|<span data-ttu-id="59bc0-184">指示检测到的登录风险的令牌颁发者的类型。</span><span class="sxs-lookup"><span data-stu-id="59bc0-184">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="59bc0-185">可取值为：`AzureAD`、`ADFederationServices`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="59bc0-185">Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="59bc0-186">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="59bc0-186">userDisplayName</span></span>|<span data-ttu-id="59bc0-187">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-187">String</span></span>|<span data-ttu-id="59bc0-188">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="59bc0-188">The user principal name (UPN) of the user.</span></span> |
|<span data-ttu-id="59bc0-189">userId</span><span class="sxs-lookup"><span data-stu-id="59bc0-189">userId</span></span>|<span data-ttu-id="59bc0-190">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-190">String</span></span>|<span data-ttu-id="59bc0-191">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="59bc0-191">Unique ID of the user.</span></span>|
|<span data-ttu-id="59bc0-192">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="59bc0-192">userPrincipalName</span></span>|<span data-ttu-id="59bc0-193">String</span><span class="sxs-lookup"><span data-stu-id="59bc0-193">String</span></span>|<span data-ttu-id="59bc0-194">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="59bc0-194">The user principal name (UPN) of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59bc0-195">关系</span><span class="sxs-lookup"><span data-stu-id="59bc0-195">Relationships</span></span>
<span data-ttu-id="59bc0-196">无。</span><span class="sxs-lookup"><span data-stu-id="59bc0-196">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59bc0-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59bc0-197">JSON representation</span></span>
<span data-ttu-id="59bc0-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59bc0-198">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "String (identifier)",
  "requestId": "String",
  "correlationId": "String",
  "riskEventType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```

