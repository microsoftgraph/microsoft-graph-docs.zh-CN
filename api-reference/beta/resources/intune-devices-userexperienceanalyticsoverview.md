---
title: userExperienceAnalyticsOverview 资源类型
description: User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 56ab161a77f21d06c034322a4daa84c5880db0da
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464984"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="aede0-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="aede0-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="aede0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aede0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aede0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aede0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aede0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aede0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aede0-107">User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="aede0-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="aede0-108">方法</span><span class="sxs-lookup"><span data-stu-id="aede0-108">Methods</span></span>
|<span data-ttu-id="aede0-109">方法</span><span class="sxs-lookup"><span data-stu-id="aede0-109">Method</span></span>|<span data-ttu-id="aede0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="aede0-110">Return Type</span></span>|<span data-ttu-id="aede0-111">说明</span><span class="sxs-lookup"><span data-stu-id="aede0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aede0-112">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="aede0-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="aede0-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="aede0-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="aede0-114">读取[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aede0-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="aede0-115">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="aede0-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="aede0-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="aede0-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="aede0-117">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aede0-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aede0-118">属性</span><span class="sxs-lookup"><span data-stu-id="aede0-118">Properties</span></span>
|<span data-ttu-id="aede0-119">属性</span><span class="sxs-lookup"><span data-stu-id="aede0-119">Property</span></span>|<span data-ttu-id="aede0-120">类型</span><span class="sxs-lookup"><span data-stu-id="aede0-120">Type</span></span>|<span data-ttu-id="aede0-121">说明</span><span class="sxs-lookup"><span data-stu-id="aede0-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aede0-122">id</span><span class="sxs-lookup"><span data-stu-id="aede0-122">id</span></span>|<span data-ttu-id="aede0-123">String</span><span class="sxs-lookup"><span data-stu-id="aede0-123">String</span></span>|<span data-ttu-id="aede0-124">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aede0-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="aede0-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="aede0-125">overallScore</span></span>|<span data-ttu-id="aede0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="aede0-126">Int32</span></span>|<span data-ttu-id="aede0-127">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="aede0-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="aede0-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="aede0-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="aede0-129">Int32</span><span class="sxs-lookup"><span data-stu-id="aede0-129">Int32</span></span>|<span data-ttu-id="aede0-130">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="aede0-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="aede0-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="aede0-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="aede0-132">Int32</span><span class="sxs-lookup"><span data-stu-id="aede0-132">Int32</span></span>|<span data-ttu-id="aede0-133">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="aede0-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="aede0-134">insights</span><span class="sxs-lookup"><span data-stu-id="aede0-134">insights</span></span>|<span data-ttu-id="aede0-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="aede0-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="aede0-136">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="aede0-136">The user experience analytics insights.</span></span>|
|<span data-ttu-id="aede0-137">state</span><span class="sxs-lookup"><span data-stu-id="aede0-137">state</span></span>|[<span data-ttu-id="aede0-138">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="aede0-138">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="aede0-139">User experience analytics 概述的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="aede0-139">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="aede0-140">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="aede0-140">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="aede0-141">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="aede0-141">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="aede0-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="aede0-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="aede0-143">User experience analytics "BootPerformance" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="aede0-143">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="aede0-144">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="aede0-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="aede0-145">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="aede0-145">bestPracticesHealthState</span></span>|[<span data-ttu-id="aede0-146">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="aede0-146">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="aede0-147">User experience analytics "BestPractices" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="aede0-147">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="aede0-148">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="aede0-148">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aede0-149">关系</span><span class="sxs-lookup"><span data-stu-id="aede0-149">Relationships</span></span>
<span data-ttu-id="aede0-150">无</span><span class="sxs-lookup"><span data-stu-id="aede0-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aede0-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aede0-151">JSON Representation</span></span>
<span data-ttu-id="aede0-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aede0-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": 1024,
  "deviceBootPerformanceOverallScore": 1024,
  "bestPracticesOverallScore": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String"
}
```



