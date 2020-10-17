---
title: riskDetection 资源类型
description: 风险检测
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb770a5d44470d1b7467001dc2d16b819a9712a4
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581293"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="2c50b-103">riskDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c50b-103">riskDetection resource type</span></span>

<span data-ttu-id="2c50b-104">命名空间： microsoft. graph 表示有关 Azure AD 租户中检测到的风险的信息。</span><span class="sxs-lookup"><span data-stu-id="2c50b-104">Namespace: microsoft.graph Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="2c50b-105">Azure AD 会根据各种信号和机器学习持续评估 [用户风险](riskyuser.md) 和应用或用户 [登录](signin.md) 风险。</span><span class="sxs-lookup"><span data-stu-id="2c50b-105">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="2c50b-106">此 API 提供对 Azure AD 环境中所有风险检测的编程访问。</span><span class="sxs-lookup"><span data-stu-id="2c50b-106">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="2c50b-107">有关风险事件的详细信息，请参阅 [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="2c50b-107">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

>[!NOTE]
><span data-ttu-id="2c50b-108">您必须具有 Azure AD 高级 P1 或 P2 许可证，才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="2c50b-108">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="2c50b-109">方法</span><span class="sxs-lookup"><span data-stu-id="2c50b-109">Methods</span></span>
|<span data-ttu-id="2c50b-110">方法</span><span class="sxs-lookup"><span data-stu-id="2c50b-110">Method</span></span>|<span data-ttu-id="2c50b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c50b-111">Return type</span></span>|<span data-ttu-id="2c50b-112">说明</span><span class="sxs-lookup"><span data-stu-id="2c50b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c50b-113">列出 riskDetections</span><span class="sxs-lookup"><span data-stu-id="2c50b-113">List riskDetections</span></span>](../api/riskdetection-list.md)|<span data-ttu-id="2c50b-114">[riskDetection](../resources/riskdetection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2c50b-114">[riskDetection](../resources/riskdetection.md) collection</span></span>|<span data-ttu-id="2c50b-115">获取 [riskDetection](../resources/riskdetection.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="2c50b-115">Get a list of the [riskDetection](../resources/riskdetection.md) objects and their properties.</span></span>|
|[<span data-ttu-id="2c50b-116">获取 riskDetection</span><span class="sxs-lookup"><span data-stu-id="2c50b-116">Get riskDetection</span></span>](../api/riskdetection-get.md)|[<span data-ttu-id="2c50b-117">riskDetection</span><span class="sxs-lookup"><span data-stu-id="2c50b-117">riskDetection</span></span>](../resources/riskdetection.md)|<span data-ttu-id="2c50b-118">读取 [riskDetection](../resources/riskdetection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c50b-118">Read the properties and relationships of a [riskDetection](../resources/riskdetection.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="2c50b-119">属性</span><span class="sxs-lookup"><span data-stu-id="2c50b-119">Properties</span></span>
|<span data-ttu-id="2c50b-120">属性</span><span class="sxs-lookup"><span data-stu-id="2c50b-120">Property</span></span>|<span data-ttu-id="2c50b-121">类型</span><span class="sxs-lookup"><span data-stu-id="2c50b-121">Type</span></span>|<span data-ttu-id="2c50b-122">说明</span><span class="sxs-lookup"><span data-stu-id="2c50b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c50b-123">activity</span><span class="sxs-lookup"><span data-stu-id="2c50b-123">activity</span></span>|<span data-ttu-id="2c50b-124">activityType</span><span class="sxs-lookup"><span data-stu-id="2c50b-124">activityType</span></span>|<span data-ttu-id="2c50b-125">指示检测到的风险所链接到的活动类型。</span><span class="sxs-lookup"><span data-stu-id="2c50b-125">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="2c50b-126">.</span><span class="sxs-lookup"><span data-stu-id="2c50b-126">.</span></span> <span data-ttu-id="2c50b-127">可取值为：`signin`、`user`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2c50b-127">Possible values are: `signin`, `user`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2c50b-128">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="2c50b-128">activityDateTime</span></span>|<span data-ttu-id="2c50b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c50b-129">DateTimeOffset</span></span>|<span data-ttu-id="2c50b-130">风险活动发生的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2c50b-130">Date and time that the risky activity occurred.</span></span>|
|<span data-ttu-id="2c50b-131">additionalInfo</span><span class="sxs-lookup"><span data-stu-id="2c50b-131">additionalInfo</span></span>|<span data-ttu-id="2c50b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="2c50b-132">String</span></span>|<span data-ttu-id="2c50b-133">与以 JSON 格式进行的风险检测相关联的其他信息。</span><span class="sxs-lookup"><span data-stu-id="2c50b-133">Additional information associated with the risk detection in JSON format.</span></span>|
|<span data-ttu-id="2c50b-134">correlationId</span><span class="sxs-lookup"><span data-stu-id="2c50b-134">correlationId</span></span>|<span data-ttu-id="2c50b-135">String</span><span class="sxs-lookup"><span data-stu-id="2c50b-135">String</span></span>|<span data-ttu-id="2c50b-136">与风险检测相关联的登录的相关 ID。</span><span class="sxs-lookup"><span data-stu-id="2c50b-136">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="2c50b-137">如果风险检测未与登录相关联，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="2c50b-137">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|<span data-ttu-id="2c50b-138">detectedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c50b-138">detectedDateTime</span></span>|<span data-ttu-id="2c50b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c50b-139">DateTimeOffset</span></span>|<span data-ttu-id="2c50b-140">检测到风险的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2c50b-140">Date and time that the risk was detected.</span></span>|
|<span data-ttu-id="2c50b-141">detectionTimingType</span><span class="sxs-lookup"><span data-stu-id="2c50b-141">detectionTimingType</span></span>|<span data-ttu-id="2c50b-142">riskDetectionTimingType</span><span class="sxs-lookup"><span data-stu-id="2c50b-142">riskDetectionTimingType</span></span>|<span data-ttu-id="2c50b-143">检测到的风险 (实时/脱机) 的时间。</span><span class="sxs-lookup"><span data-stu-id="2c50b-143">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="2c50b-144">可取值为：`notDefined`、`realtime`、`nearRealtime`、`offline`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2c50b-144">Possible values are: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2c50b-145">id</span><span class="sxs-lookup"><span data-stu-id="2c50b-145">id</span></span>|<span data-ttu-id="2c50b-146">字符串</span><span class="sxs-lookup"><span data-stu-id="2c50b-146">String</span></span>|<span data-ttu-id="2c50b-147">风险检测的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2c50b-147">Unique ID of the risk detection.</span></span> <span data-ttu-id="2c50b-148">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="2c50b-148">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="2c50b-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2c50b-149">ipAddress</span></span>|<span data-ttu-id="2c50b-150">String</span><span class="sxs-lookup"><span data-stu-id="2c50b-150">String</span></span>|<span data-ttu-id="2c50b-151">提供从其发生风险的客户端的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="2c50b-151">Provides the IP address of the client from where the risk occurred.</span></span>|
|<span data-ttu-id="2c50b-152">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c50b-152">lastUpdatedDateTime</span></span>|<span data-ttu-id="2c50b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c50b-153">DateTimeOffset</span></span>|<span data-ttu-id="2c50b-154">上次更新风险检测的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2c50b-154">Date and time that the risk detection was last updated.</span></span>|
|<span data-ttu-id="2c50b-155">location</span><span class="sxs-lookup"><span data-stu-id="2c50b-155">location</span></span>|[<span data-ttu-id="2c50b-156">signInLocation</span><span class="sxs-lookup"><span data-stu-id="2c50b-156">signInLocation</span></span>](../resources/signinlocation.md)|<span data-ttu-id="2c50b-157">登录的位置。</span><span class="sxs-lookup"><span data-stu-id="2c50b-157">Location of the sign-in.</span></span>|
|<span data-ttu-id="2c50b-158">请求</span><span class="sxs-lookup"><span data-stu-id="2c50b-158">requestId</span></span>|<span data-ttu-id="2c50b-159">字符串</span><span class="sxs-lookup"><span data-stu-id="2c50b-159">String</span></span>|<span data-ttu-id="2c50b-160">与风险检测相关联的登录请求 ID。</span><span class="sxs-lookup"><span data-stu-id="2c50b-160">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="2c50b-161">如果风险检测未与登录相关联，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="2c50b-161">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|<span data-ttu-id="2c50b-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2c50b-162">riskDetail</span></span>|<span data-ttu-id="2c50b-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2c50b-163">riskDetail</span></span>|<span data-ttu-id="2c50b-164">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2c50b-164">Details of the detected risk.</span></span> <span data-ttu-id="2c50b-165">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2c50b-165">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2c50b-166">riskEventType</span><span class="sxs-lookup"><span data-stu-id="2c50b-166">riskEventType</span></span>|<span data-ttu-id="2c50b-167">字符串</span><span class="sxs-lookup"><span data-stu-id="2c50b-167">String</span></span>|<span data-ttu-id="2c50b-168">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="2c50b-168">The type of risk event detected.</span></span> <span data-ttu-id="2c50b-169">可能的值为、、、、、、、、、、、、 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` 和 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="2c50b-169">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> <span data-ttu-id="2c50b-170">如果风险检测是高级检测，将显示 `generic`</span><span class="sxs-lookup"><span data-stu-id="2c50b-170">If the risk detection is a premium detection, will show `generic`</span></span>|
|<span data-ttu-id="2c50b-171">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2c50b-171">riskLevel</span></span>|<span data-ttu-id="2c50b-172">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2c50b-172">riskLevel</span></span>|<span data-ttu-id="2c50b-173">检测到的风险的级别。</span><span class="sxs-lookup"><span data-stu-id="2c50b-173">Level of the detected risk.</span></span> <span data-ttu-id="2c50b-174">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2c50b-174">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2c50b-175">riskState</span><span class="sxs-lookup"><span data-stu-id="2c50b-175">riskState</span></span>|<span data-ttu-id="2c50b-176">riskState</span><span class="sxs-lookup"><span data-stu-id="2c50b-176">riskState</span></span>|<span data-ttu-id="2c50b-177">检测到的有风险的用户或登录的状态。</span><span class="sxs-lookup"><span data-stu-id="2c50b-177">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="2c50b-178">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2c50b-178">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2c50b-179">source</span><span class="sxs-lookup"><span data-stu-id="2c50b-179">source</span></span>|<span data-ttu-id="2c50b-180">字符串</span><span class="sxs-lookup"><span data-stu-id="2c50b-180">String</span></span>|<span data-ttu-id="2c50b-181">风险检测的来源。</span><span class="sxs-lookup"><span data-stu-id="2c50b-181">Source of the risk detection.</span></span> <span data-ttu-id="2c50b-182">例如，"activeDirectory"。</span><span class="sxs-lookup"><span data-stu-id="2c50b-182">For example, "activeDirectory".</span></span> |
|<span data-ttu-id="2c50b-183">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="2c50b-183">tokenIssuerType</span></span>|<span data-ttu-id="2c50b-184">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="2c50b-184">tokenIssuerType</span></span>|<span data-ttu-id="2c50b-185">指示检测到的登录风险的令牌颁发者的类型。</span><span class="sxs-lookup"><span data-stu-id="2c50b-185">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="2c50b-186">可取值为：`AzureAD`、`ADFederationServices`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2c50b-186">Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="2c50b-187">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2c50b-187">userDisplayName</span></span>|<span data-ttu-id="2c50b-188">String</span><span class="sxs-lookup"><span data-stu-id="2c50b-188">String</span></span>|<span data-ttu-id="2c50b-189">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="2c50b-189">The user principal name (UPN) of the user.</span></span> |
|<span data-ttu-id="2c50b-190">userId</span><span class="sxs-lookup"><span data-stu-id="2c50b-190">userId</span></span>|<span data-ttu-id="2c50b-191">字符串</span><span class="sxs-lookup"><span data-stu-id="2c50b-191">String</span></span>|<span data-ttu-id="2c50b-192">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2c50b-192">Unique ID of the user.</span></span>|
|<span data-ttu-id="2c50b-193">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2c50b-193">userPrincipalName</span></span>|<span data-ttu-id="2c50b-194">String</span><span class="sxs-lookup"><span data-stu-id="2c50b-194">String</span></span>|<span data-ttu-id="2c50b-195">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="2c50b-195">The user principal name (UPN) of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c50b-196">关系</span><span class="sxs-lookup"><span data-stu-id="2c50b-196">Relationships</span></span>
<span data-ttu-id="2c50b-197">无。</span><span class="sxs-lookup"><span data-stu-id="2c50b-197">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c50b-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c50b-198">JSON representation</span></span>
<span data-ttu-id="2c50b-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c50b-199">The following is a JSON representation of the resource.</span></span>
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