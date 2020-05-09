---
title: userExperienceAnalyticsOverview 资源类型
description: User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 152f5ef93db38ffced60bf93e3215d45cf822ba5
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175516"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="65ca6-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="65ca6-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="65ca6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65ca6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65ca6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65ca6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65ca6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65ca6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65ca6-107">User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="65ca6-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="65ca6-108">方法</span><span class="sxs-lookup"><span data-stu-id="65ca6-108">Methods</span></span>
|<span data-ttu-id="65ca6-109">方法</span><span class="sxs-lookup"><span data-stu-id="65ca6-109">Method</span></span>|<span data-ttu-id="65ca6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="65ca6-110">Return Type</span></span>|<span data-ttu-id="65ca6-111">说明</span><span class="sxs-lookup"><span data-stu-id="65ca6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65ca6-112">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="65ca6-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="65ca6-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="65ca6-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="65ca6-114">读取[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="65ca6-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="65ca6-115">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="65ca6-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="65ca6-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="65ca6-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="65ca6-117">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="65ca6-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="65ca6-118">属性</span><span class="sxs-lookup"><span data-stu-id="65ca6-118">Properties</span></span>
|<span data-ttu-id="65ca6-119">属性</span><span class="sxs-lookup"><span data-stu-id="65ca6-119">Property</span></span>|<span data-ttu-id="65ca6-120">类型</span><span class="sxs-lookup"><span data-stu-id="65ca6-120">Type</span></span>|<span data-ttu-id="65ca6-121">说明</span><span class="sxs-lookup"><span data-stu-id="65ca6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65ca6-122">id</span><span class="sxs-lookup"><span data-stu-id="65ca6-122">id</span></span>|<span data-ttu-id="65ca6-123">字符串</span><span class="sxs-lookup"><span data-stu-id="65ca6-123">String</span></span>|<span data-ttu-id="65ca6-124">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="65ca6-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="65ca6-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="65ca6-125">overallScore</span></span>|<span data-ttu-id="65ca6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="65ca6-126">Int32</span></span>|<span data-ttu-id="65ca6-127">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="65ca6-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="65ca6-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="65ca6-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="65ca6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="65ca6-129">Int32</span></span>|<span data-ttu-id="65ca6-130">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="65ca6-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="65ca6-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="65ca6-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="65ca6-132">Int32</span><span class="sxs-lookup"><span data-stu-id="65ca6-132">Int32</span></span>|<span data-ttu-id="65ca6-133">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="65ca6-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="65ca6-134">insights</span><span class="sxs-lookup"><span data-stu-id="65ca6-134">insights</span></span>|<span data-ttu-id="65ca6-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="65ca6-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="65ca6-136">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="65ca6-136">The user experience analytics insights.</span></span>|
|<span data-ttu-id="65ca6-137">state</span><span class="sxs-lookup"><span data-stu-id="65ca6-137">state</span></span>|[<span data-ttu-id="65ca6-138">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="65ca6-138">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="65ca6-139">User experience analytics 概述的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="65ca6-139">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="65ca6-140">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="65ca6-140">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="65ca6-141">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="65ca6-141">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="65ca6-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="65ca6-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="65ca6-143">User experience analytics "BootPerformance" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="65ca6-143">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="65ca6-144">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="65ca6-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="65ca6-145">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="65ca6-145">bestPracticesHealthState</span></span>|[<span data-ttu-id="65ca6-146">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="65ca6-146">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="65ca6-147">User experience analytics "BestPractices" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="65ca6-147">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="65ca6-148">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="65ca6-148">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65ca6-149">关系</span><span class="sxs-lookup"><span data-stu-id="65ca6-149">Relationships</span></span>
<span data-ttu-id="65ca6-150">无</span><span class="sxs-lookup"><span data-stu-id="65ca6-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65ca6-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65ca6-151">JSON Representation</span></span>
<span data-ttu-id="65ca6-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65ca6-152">Here is a JSON representation of the resource.</span></span>
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
          "value": "4.2"
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



