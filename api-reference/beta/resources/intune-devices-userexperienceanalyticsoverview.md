---
title: userExperienceAnalyticsOverview 资源类型
description: 用户体验分析概述实体包含所有类别的总体分数以及每个指标的分数和见解。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32466ea9fa14efe0c46b812ac1f6babc9ba32102
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866550"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="06f79-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="06f79-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="06f79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06f79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06f79-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06f79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06f79-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06f79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06f79-107">用户体验分析概述实体包含所有类别的总体分数以及每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="06f79-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="06f79-108">方法</span><span class="sxs-lookup"><span data-stu-id="06f79-108">Methods</span></span>
|<span data-ttu-id="06f79-109">方法</span><span class="sxs-lookup"><span data-stu-id="06f79-109">Method</span></span>|<span data-ttu-id="06f79-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="06f79-110">Return Type</span></span>|<span data-ttu-id="06f79-111">说明</span><span class="sxs-lookup"><span data-stu-id="06f79-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06f79-112">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="06f79-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="06f79-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="06f79-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="06f79-114">读取 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06f79-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="06f79-115">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="06f79-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="06f79-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="06f79-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="06f79-117">更新 [userExperienceAnalyticsOverview 对象](../resources/intune-devices-userexperienceanalyticsoverview.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="06f79-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06f79-118">属性</span><span class="sxs-lookup"><span data-stu-id="06f79-118">Properties</span></span>
|<span data-ttu-id="06f79-119">属性</span><span class="sxs-lookup"><span data-stu-id="06f79-119">Property</span></span>|<span data-ttu-id="06f79-120">类型</span><span class="sxs-lookup"><span data-stu-id="06f79-120">Type</span></span>|<span data-ttu-id="06f79-121">说明</span><span class="sxs-lookup"><span data-stu-id="06f79-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06f79-122">id</span><span class="sxs-lookup"><span data-stu-id="06f79-122">id</span></span>|<span data-ttu-id="06f79-123">String</span><span class="sxs-lookup"><span data-stu-id="06f79-123">String</span></span>|<span data-ttu-id="06f79-124">用户体验分析概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="06f79-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="06f79-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="06f79-125">overallScore</span></span>|<span data-ttu-id="06f79-126">Int32</span><span class="sxs-lookup"><span data-stu-id="06f79-126">Int32</span></span>|<span data-ttu-id="06f79-127">用户体验分析总体分数。</span><span class="sxs-lookup"><span data-stu-id="06f79-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="06f79-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="06f79-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="06f79-129">Int32</span><span class="sxs-lookup"><span data-stu-id="06f79-129">Int32</span></span>|<span data-ttu-id="06f79-130">用户体验分析设备启动性能总体分数。</span><span class="sxs-lookup"><span data-stu-id="06f79-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="06f79-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="06f79-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="06f79-132">Int32</span><span class="sxs-lookup"><span data-stu-id="06f79-132">Int32</span></span>|<span data-ttu-id="06f79-133">用户体验分析最佳实践总体分数。</span><span class="sxs-lookup"><span data-stu-id="06f79-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="06f79-134">workFromAnywhereOverallScore</span><span class="sxs-lookup"><span data-stu-id="06f79-134">workFromAnywhereOverallScore</span></span>|<span data-ttu-id="06f79-135">Int32</span><span class="sxs-lookup"><span data-stu-id="06f79-135">Int32</span></span>|<span data-ttu-id="06f79-136">用户体验分析从任意位置工作总体分数。</span><span class="sxs-lookup"><span data-stu-id="06f79-136">The user experience analytics Work From Anywhere overall score.</span></span>|
|<span data-ttu-id="06f79-137">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="06f79-137">appHealthOverallScore</span></span>|<span data-ttu-id="06f79-138">Int32</span><span class="sxs-lookup"><span data-stu-id="06f79-138">Int32</span></span>|<span data-ttu-id="06f79-139">用户体验分析应用运行状况总体分数。</span><span class="sxs-lookup"><span data-stu-id="06f79-139">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="06f79-140">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="06f79-140">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="06f79-141">Int32</span><span class="sxs-lookup"><span data-stu-id="06f79-141">Int32</span></span>|<span data-ttu-id="06f79-142">用户体验分析资源性能总体分数。</span><span class="sxs-lookup"><span data-stu-id="06f79-142">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="06f79-143">insights</span><span class="sxs-lookup"><span data-stu-id="06f79-143">insights</span></span>|<span data-ttu-id="06f79-144">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06f79-144">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="06f79-145">用户体验分析见解。</span><span class="sxs-lookup"><span data-stu-id="06f79-145">The user experience analytics insights.</span></span>|
|<span data-ttu-id="06f79-146">state</span><span class="sxs-lookup"><span data-stu-id="06f79-146">state</span></span>|[<span data-ttu-id="06f79-147">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-147">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="06f79-148">用户体验分析概述的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="06f79-148">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="06f79-149">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="06f79-149">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="06f79-150">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-150">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="06f79-151">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-151">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="06f79-152">用户体验分析"BootPerformance"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="06f79-152">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="06f79-153">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="06f79-153">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="06f79-154">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-154">bestPracticesHealthState</span></span>|[<span data-ttu-id="06f79-155">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-155">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="06f79-156">用户体验分析"BestPractices"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="06f79-156">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="06f79-157">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="06f79-157">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="06f79-158">workFromAnywhereHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-158">workFromAnywhereHealthState</span></span>|[<span data-ttu-id="06f79-159">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-159">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="06f79-160">用户体验分析"WorkFromAnywhere"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="06f79-160">The current health state of the user experience analytics 'WorkFromAnywhere' category.</span></span> <span data-ttu-id="06f79-161">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="06f79-161">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="06f79-162">appHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-162">appHealthState</span></span>|[<span data-ttu-id="06f79-163">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-163">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="06f79-164">用户体验分析"BestPractices"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="06f79-164">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="06f79-165">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="06f79-165">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="06f79-166">resourcePerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-166">resourcePerformanceHealthState</span></span>|[<span data-ttu-id="06f79-167">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="06f79-167">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="06f79-168">用户体验分析"ResourcePerformance"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="06f79-168">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="06f79-169">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="06f79-169">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06f79-170">关系</span><span class="sxs-lookup"><span data-stu-id="06f79-170">Relationships</span></span>
<span data-ttu-id="06f79-171">无</span><span class="sxs-lookup"><span data-stu-id="06f79-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06f79-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06f79-172">JSON Representation</span></span>
<span data-ttu-id="06f79-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06f79-173">Here is a JSON representation of the resource.</span></span>
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
  "workFromAnywhereOverallScore": 1024,
  "appHealthOverallScore": 1024,
  "resourcePerformanceOverallScore": 1024,
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
  "bestPracticesHealthState": "String",
  "workFromAnywhereHealthState": "String",
  "appHealthState": "String",
  "resourcePerformanceHealthState": "String"
}
```




