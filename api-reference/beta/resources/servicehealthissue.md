---
title: serviceHealthIssue 资源类型
description: 表示服务中的服务运行状况问题。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 2436e6d0d5e49155b936cbfb7f7fc98630b7ce57
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109095"
---
# <a name="servicehealthissue-resource-type"></a><span data-ttu-id="0d0c0-103">serviceHealthIssue 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d0c0-103">serviceHealthIssue resource type</span></span>

<span data-ttu-id="0d0c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d0c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d0c0-105">表示服务中的服务运行状况问题。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-105">Represents a service health issue in a service.</span></span>

<span data-ttu-id="0d0c0-106">服务运行状况问题可以是服务事件或服务公告。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-106">The service health issue can be a service incident or service advisory.</span></span> <span data-ttu-id="0d0c0-107">例如：</span><span class="sxs-lookup"><span data-stu-id="0d0c0-107">For example:</span></span>

* <span data-ttu-id="0d0c0-108">服务事件："Exchange邮箱服务关闭"。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-108">Service incident: "Exchange mailbox service is down".</span></span>
* <span data-ttu-id="0d0c0-109">服务公告："用户在接收电子邮件时可能会遇到延迟"。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-109">Service advisory: "Users may experience delays in emails reception".</span></span>

<span data-ttu-id="0d0c0-110">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-110">Inherits from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0d0c0-111">方法</span><span class="sxs-lookup"><span data-stu-id="0d0c0-111">Methods</span></span>
|<span data-ttu-id="0d0c0-112">方法</span><span class="sxs-lookup"><span data-stu-id="0d0c0-112">Method</span></span>|<span data-ttu-id="0d0c0-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="0d0c0-113">Return type</span></span>|<span data-ttu-id="0d0c0-114">说明</span><span class="sxs-lookup"><span data-stu-id="0d0c0-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0d0c0-115">获取 serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="0d0c0-115">Get serviceHealthIssue</span></span>](../api/servicehealthissue-get.md)|[<span data-ttu-id="0d0c0-116">serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="0d0c0-116">serviceHealthIssue</span></span>](../resources/servicehealthissue.md)|<span data-ttu-id="0d0c0-117">检索 [serviceHealthIssue](../resources/servicehealthissue.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-117">Retrieve the properties and relationships of a [serviceHealthIssue](../resources/servicehealthissue.md) object.</span></span> |
|[<span data-ttu-id="0d0c0-118">获取事后评审报告</span><span class="sxs-lookup"><span data-stu-id="0d0c0-118">Get post-incident review report</span></span>](../api/servicehealthissue-incidentreport.md)|<span data-ttu-id="0d0c0-119">Stream</span><span class="sxs-lookup"><span data-stu-id="0d0c0-119">Stream</span></span>|<span data-ttu-id="0d0c0-120">提供事件后报告 (PIR) 租户的指定服务问题的文档。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-120">Provides the post incident report (PIR) document of a specified service issue for tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d0c0-121">属性</span><span class="sxs-lookup"><span data-stu-id="0d0c0-121">Properties</span></span>
|<span data-ttu-id="0d0c0-122">属性</span><span class="sxs-lookup"><span data-stu-id="0d0c0-122">Property</span></span>|<span data-ttu-id="0d0c0-123">类型</span><span class="sxs-lookup"><span data-stu-id="0d0c0-123">Type</span></span>|<span data-ttu-id="0d0c0-124">说明</span><span class="sxs-lookup"><span data-stu-id="0d0c0-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d0c0-125">classification</span><span class="sxs-lookup"><span data-stu-id="0d0c0-125">classification</span></span>|<span data-ttu-id="0d0c0-126">serviceHealthClassificationType</span><span class="sxs-lookup"><span data-stu-id="0d0c0-126">serviceHealthClassificationType</span></span>|<span data-ttu-id="0d0c0-127">服务运行状况问题的类型。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-127">The type of service health issue.</span></span> <span data-ttu-id="0d0c0-128">可取值为：`advisory`、`incident`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-128">Possible values are: `advisory`, `incident`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0d0c0-129">详细信息</span><span class="sxs-lookup"><span data-stu-id="0d0c0-129">details</span></span>|<span data-ttu-id="0d0c0-130">collection ([keyValuePair](../resources/keyvaluepair.md)) </span><span class="sxs-lookup"><span data-stu-id="0d0c0-130">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="0d0c0-131">有关服务运行状况问题的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-131">Additional details about service health issue.</span></span> <span data-ttu-id="0d0c0-132">此属性不支持筛选器。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-132">This property doesn't support filters.</span></span> <span data-ttu-id="0d0c0-133">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-133">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="0d0c0-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0d0c0-134">endDateTime</span></span>|<span data-ttu-id="0d0c0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d0c0-135">DateTimeOffset</span></span>|<span data-ttu-id="0d0c0-136">服务问题的结束时间。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-136">The end time of the service issue.</span></span> <span data-ttu-id="0d0c0-137">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-137">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="0d0c0-138">功能</span><span class="sxs-lookup"><span data-stu-id="0d0c0-138">feature</span></span>|<span data-ttu-id="0d0c0-139">字符串</span><span class="sxs-lookup"><span data-stu-id="0d0c0-139">String</span></span>|<span data-ttu-id="0d0c0-140">服务问题的功能名称。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-140">The feature name of the service issue.</span></span>|
|<span data-ttu-id="0d0c0-141">featureGroup</span><span class="sxs-lookup"><span data-stu-id="0d0c0-141">featureGroup</span></span>|<span data-ttu-id="0d0c0-142">字符串</span><span class="sxs-lookup"><span data-stu-id="0d0c0-142">String</span></span>|<span data-ttu-id="0d0c0-143">服务问题的功能组名称。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-143">The feature group name of the service issue.</span></span>|
|<span data-ttu-id="0d0c0-144">id</span><span class="sxs-lookup"><span data-stu-id="0d0c0-144">id</span></span>|<span data-ttu-id="0d0c0-145">字符串</span><span class="sxs-lookup"><span data-stu-id="0d0c0-145">String</span></span>|<span data-ttu-id="0d0c0-146">服务问题的 ID。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-146">The id of the service issue.</span></span> <span data-ttu-id="0d0c0-147">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-147">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="0d0c0-148">impactDescription</span><span class="sxs-lookup"><span data-stu-id="0d0c0-148">impactDescription</span></span>|<span data-ttu-id="0d0c0-149">字符串</span><span class="sxs-lookup"><span data-stu-id="0d0c0-149">String</span></span>|<span data-ttu-id="0d0c0-150">服务问题影响的说明。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-150">The description of the service issue impact.</span></span>|
|<span data-ttu-id="0d0c0-151">isResolved</span><span class="sxs-lookup"><span data-stu-id="0d0c0-151">isResolved</span></span>|<span data-ttu-id="0d0c0-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="0d0c0-152">Boolean</span></span>|<span data-ttu-id="0d0c0-153">指示该问题是否已解决。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-153">Indicates whether the issue is resolved.</span></span>|
|<span data-ttu-id="0d0c0-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d0c0-154">lastModifiedDateTime</span></span>|<span data-ttu-id="0d0c0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d0c0-155">DateTimeOffset</span></span>|<span data-ttu-id="0d0c0-156">问题的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-156">The last modified time of the issue.</span></span> <span data-ttu-id="0d0c0-157">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-157">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="0d0c0-158">origin</span><span class="sxs-lookup"><span data-stu-id="0d0c0-158">origin</span></span>|<span data-ttu-id="0d0c0-159">serviceHealthOrigin</span><span class="sxs-lookup"><span data-stu-id="0d0c0-159">serviceHealthOrigin</span></span>|<span data-ttu-id="0d0c0-160">指示服务问题的来源。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-160">Indicates the origin of the service issue.</span></span> <span data-ttu-id="0d0c0-161">可取值为：`microsoft`、`thirdParty`、`customer`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-161">Possible values are: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0d0c0-162">公告</span><span class="sxs-lookup"><span data-stu-id="0d0c0-162">posts</span></span>|<span data-ttu-id="0d0c0-163">collection ([serviceHealthIssuePost](../resources/servicehealthissuepost.md)) </span><span class="sxs-lookup"><span data-stu-id="0d0c0-163">Collection([serviceHealthIssuePost](../resources/servicehealthissuepost.md))</span></span>|<span data-ttu-id="0d0c0-164">服务问题的历史文章集合。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-164">Collection of historical posts for the service issue.</span></span>|
|<span data-ttu-id="0d0c0-165">service</span><span class="sxs-lookup"><span data-stu-id="0d0c0-165">service</span></span>|<span data-ttu-id="0d0c0-166">String</span><span class="sxs-lookup"><span data-stu-id="0d0c0-166">String</span></span>|<span data-ttu-id="0d0c0-167">指示受问题影响的服务。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-167">Indicates the service affected by the issue.</span></span>|
|<span data-ttu-id="0d0c0-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d0c0-168">startDateTime</span></span>|<span data-ttu-id="0d0c0-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d0c0-169">DateTimeOffset</span></span>|<span data-ttu-id="0d0c0-170">服务问题的开始时间。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-170">The start time of the service issue.</span></span> <span data-ttu-id="0d0c0-171">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-171">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="0d0c0-172">状态</span><span class="sxs-lookup"><span data-stu-id="0d0c0-172">status</span></span>|<span data-ttu-id="0d0c0-173">serviceHealthStatus</span><span class="sxs-lookup"><span data-stu-id="0d0c0-173">serviceHealthStatus</span></span>|<span data-ttu-id="0d0c0-174">服务问题的状态。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-174">The status of the service issue.</span></span> <span data-ttu-id="0d0c0-175">可能的值是 `serviceOperational` `investigating` `restoringService` ：、、、、、、、、、 `verifyingService` `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-175">Possible values are: `serviceOperational`, `investigating`, `restoringService`, `verifyingService`, `serviceRestored`, `postIncidentReviewPublished`, `serviceDegradation`, `serviceInterruption`, `extendedRecovery`, `falsePositive`, `investigationSuspended`, `resolved`, `mitigatedExternal`, `mitigated`, `resolvedExternal`, `confirmed`, `reported`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0d0c0-176">title</span><span class="sxs-lookup"><span data-stu-id="0d0c0-176">title</span></span>|<span data-ttu-id="0d0c0-177">String</span><span class="sxs-lookup"><span data-stu-id="0d0c0-177">String</span></span>|<span data-ttu-id="0d0c0-178">服务问题的标题。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-178">The title of the service issue.</span></span> <span data-ttu-id="0d0c0-179">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-179">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d0c0-180">关系</span><span class="sxs-lookup"><span data-stu-id="0d0c0-180">Relationships</span></span>
<span data-ttu-id="0d0c0-181">无。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d0c0-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d0c0-182">JSON representation</span></span>
<span data-ttu-id="0d0c0-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d0c0-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssue",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "impactDescription": "String",
  "classification": "String",
  "origin": "String",
  "posts": [
    {
      "@odata.type": "microsoft.graph.serviceHealthIssuePost"
    }
  ],
  "status": "String",
  "service": "String",
  "feature": "String",
  "featureGroup": "String",
  "isResolved": "Boolean"
}
```

