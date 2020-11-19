---
title: userExperienceAnalyticsOverview 资源类型
description: User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b64aa5f0a55024425a3feab4105d7f2ccaf8f39
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256397"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="42520-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="42520-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="42520-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42520-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42520-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42520-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42520-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42520-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42520-107">User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="42520-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="42520-108">方法</span><span class="sxs-lookup"><span data-stu-id="42520-108">Methods</span></span>
|<span data-ttu-id="42520-109">方法</span><span class="sxs-lookup"><span data-stu-id="42520-109">Method</span></span>|<span data-ttu-id="42520-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="42520-110">Return Type</span></span>|<span data-ttu-id="42520-111">说明</span><span class="sxs-lookup"><span data-stu-id="42520-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42520-112">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="42520-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="42520-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="42520-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="42520-114">读取 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="42520-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="42520-115">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="42520-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="42520-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="42520-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="42520-117">更新 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="42520-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="42520-118">属性</span><span class="sxs-lookup"><span data-stu-id="42520-118">Properties</span></span>
|<span data-ttu-id="42520-119">属性</span><span class="sxs-lookup"><span data-stu-id="42520-119">Property</span></span>|<span data-ttu-id="42520-120">类型</span><span class="sxs-lookup"><span data-stu-id="42520-120">Type</span></span>|<span data-ttu-id="42520-121">说明</span><span class="sxs-lookup"><span data-stu-id="42520-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42520-122">id</span><span class="sxs-lookup"><span data-stu-id="42520-122">id</span></span>|<span data-ttu-id="42520-123">String</span><span class="sxs-lookup"><span data-stu-id="42520-123">String</span></span>|<span data-ttu-id="42520-124">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="42520-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="42520-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="42520-125">overallScore</span></span>|<span data-ttu-id="42520-126">Int32</span><span class="sxs-lookup"><span data-stu-id="42520-126">Int32</span></span>|<span data-ttu-id="42520-127">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="42520-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="42520-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="42520-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="42520-129">Int32</span><span class="sxs-lookup"><span data-stu-id="42520-129">Int32</span></span>|<span data-ttu-id="42520-130">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="42520-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="42520-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="42520-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="42520-132">Int32</span><span class="sxs-lookup"><span data-stu-id="42520-132">Int32</span></span>|<span data-ttu-id="42520-133">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="42520-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="42520-134">insights</span><span class="sxs-lookup"><span data-stu-id="42520-134">insights</span></span>|<span data-ttu-id="42520-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42520-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="42520-136">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="42520-136">The user experience analytics insights.</span></span>|
|<span data-ttu-id="42520-137">state</span><span class="sxs-lookup"><span data-stu-id="42520-137">state</span></span>|[<span data-ttu-id="42520-138">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="42520-138">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="42520-139">User experience analytics 概述的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="42520-139">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="42520-140">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="42520-140">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="42520-141">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="42520-141">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="42520-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="42520-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="42520-143">User experience analytics "BootPerformance" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="42520-143">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="42520-144">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="42520-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="42520-145">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="42520-145">bestPracticesHealthState</span></span>|[<span data-ttu-id="42520-146">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="42520-146">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="42520-147">User experience analytics "BestPractices" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="42520-147">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="42520-148">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="42520-148">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42520-149">关系</span><span class="sxs-lookup"><span data-stu-id="42520-149">Relationships</span></span>
<span data-ttu-id="42520-150">无</span><span class="sxs-lookup"><span data-stu-id="42520-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42520-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42520-151">JSON Representation</span></span>
<span data-ttu-id="42520-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42520-152">Here is a JSON representation of the resource.</span></span>
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




