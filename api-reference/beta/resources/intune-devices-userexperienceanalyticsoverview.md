---
title: userExperienceAnalyticsOverview 资源类型
description: 用户体验分析概述实体包含所有类别的所有指标的整体分数和分数和见解。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 655eedf3cfab990c6c83998ff7c0fd3ae78b6dff
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159547"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="6e7ef-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e7ef-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="6e7ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e7ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e7ef-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e7ef-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e7ef-107">用户体验分析概述实体包含所有类别的所有指标的整体分数和分数和见解。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="6e7ef-108">方法</span><span class="sxs-lookup"><span data-stu-id="6e7ef-108">Methods</span></span>
|<span data-ttu-id="6e7ef-109">方法</span><span class="sxs-lookup"><span data-stu-id="6e7ef-109">Method</span></span>|<span data-ttu-id="6e7ef-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6e7ef-110">Return Type</span></span>|<span data-ttu-id="6e7ef-111">说明</span><span class="sxs-lookup"><span data-stu-id="6e7ef-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e7ef-112">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="6e7ef-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="6e7ef-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="6e7ef-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="6e7ef-114">读取 [userExperienceAnalyticsOverview 对象的属性和](../resources/intune-devices-userexperienceanalyticsoverview.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="6e7ef-115">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="6e7ef-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="6e7ef-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="6e7ef-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="6e7ef-117">更新 [userExperienceAnalyticsOverview 对象](../resources/intune-devices-userexperienceanalyticsoverview.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e7ef-118">属性</span><span class="sxs-lookup"><span data-stu-id="6e7ef-118">Properties</span></span>
|<span data-ttu-id="6e7ef-119">属性</span><span class="sxs-lookup"><span data-stu-id="6e7ef-119">Property</span></span>|<span data-ttu-id="6e7ef-120">类型</span><span class="sxs-lookup"><span data-stu-id="6e7ef-120">Type</span></span>|<span data-ttu-id="6e7ef-121">说明</span><span class="sxs-lookup"><span data-stu-id="6e7ef-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e7ef-122">id</span><span class="sxs-lookup"><span data-stu-id="6e7ef-122">id</span></span>|<span data-ttu-id="6e7ef-123">String</span><span class="sxs-lookup"><span data-stu-id="6e7ef-123">String</span></span>|<span data-ttu-id="6e7ef-124">用户体验分析概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="6e7ef-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="6e7ef-125">overallScore</span></span>|<span data-ttu-id="6e7ef-126">Int32</span><span class="sxs-lookup"><span data-stu-id="6e7ef-126">Int32</span></span>|<span data-ttu-id="6e7ef-127">用户体验分析总体分数。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="6e7ef-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="6e7ef-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="6e7ef-129">Int32</span><span class="sxs-lookup"><span data-stu-id="6e7ef-129">Int32</span></span>|<span data-ttu-id="6e7ef-130">用户体验分析设备启动性能总体分数。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="6e7ef-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="6e7ef-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="6e7ef-132">Int32</span><span class="sxs-lookup"><span data-stu-id="6e7ef-132">Int32</span></span>|<span data-ttu-id="6e7ef-133">用户体验分析最佳做法总体分数。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="6e7ef-134">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="6e7ef-134">appHealthOverallScore</span></span>|<span data-ttu-id="6e7ef-135">Int32</span><span class="sxs-lookup"><span data-stu-id="6e7ef-135">Int32</span></span>|<span data-ttu-id="6e7ef-136">用户体验分析应用运行状况总体分数。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-136">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="6e7ef-137">insights</span><span class="sxs-lookup"><span data-stu-id="6e7ef-137">insights</span></span>|<span data-ttu-id="6e7ef-138">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6e7ef-138">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="6e7ef-139">用户体验分析见解。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-139">The user experience analytics insights.</span></span>|
|<span data-ttu-id="6e7ef-140">state</span><span class="sxs-lookup"><span data-stu-id="6e7ef-140">state</span></span>|[<span data-ttu-id="6e7ef-141">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6e7ef-141">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6e7ef-142">用户体验分析概述的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-142">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="6e7ef-143">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-143">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6e7ef-144">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="6e7ef-144">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="6e7ef-145">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6e7ef-145">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6e7ef-146">用户体验分析"BootPerformance"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-146">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="6e7ef-147">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-147">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6e7ef-148">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="6e7ef-148">bestPracticesHealthState</span></span>|[<span data-ttu-id="6e7ef-149">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6e7ef-149">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6e7ef-150">用户体验分析"BestPractices"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-150">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="6e7ef-151">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-151">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6e7ef-152">appHealthState</span><span class="sxs-lookup"><span data-stu-id="6e7ef-152">appHealthState</span></span>|[<span data-ttu-id="6e7ef-153">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6e7ef-153">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6e7ef-154">用户体验分析"BestPractices"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-154">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="6e7ef-155">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-155">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e7ef-156">关系</span><span class="sxs-lookup"><span data-stu-id="6e7ef-156">Relationships</span></span>
<span data-ttu-id="6e7ef-157">无</span><span class="sxs-lookup"><span data-stu-id="6e7ef-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e7ef-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e7ef-158">JSON Representation</span></span>
<span data-ttu-id="6e7ef-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e7ef-159">Here is a JSON representation of the resource.</span></span>
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
  "appHealthOverallScore": 1024,
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
  "appHealthState": "String"
}
```




