---
title: userExperienceAnalyticsOverview 资源类型
description: User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 306c6c9e2ca1903c2bd16012dba3b78e1c906cd6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783765"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="c6d52-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6d52-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="c6d52-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6d52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6d52-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6d52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6d52-106">User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="c6d52-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="c6d52-107">方法</span><span class="sxs-lookup"><span data-stu-id="c6d52-107">Methods</span></span>
|<span data-ttu-id="c6d52-108">方法</span><span class="sxs-lookup"><span data-stu-id="c6d52-108">Method</span></span>|<span data-ttu-id="c6d52-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6d52-109">Return Type</span></span>|<span data-ttu-id="c6d52-110">说明</span><span class="sxs-lookup"><span data-stu-id="c6d52-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6d52-111">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="c6d52-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="c6d52-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="c6d52-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="c6d52-113">读取[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6d52-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="c6d52-114">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="c6d52-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="c6d52-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="c6d52-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="c6d52-116">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c6d52-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6d52-117">属性</span><span class="sxs-lookup"><span data-stu-id="c6d52-117">Properties</span></span>
|<span data-ttu-id="c6d52-118">属性</span><span class="sxs-lookup"><span data-stu-id="c6d52-118">Property</span></span>|<span data-ttu-id="c6d52-119">类型</span><span class="sxs-lookup"><span data-stu-id="c6d52-119">Type</span></span>|<span data-ttu-id="c6d52-120">说明</span><span class="sxs-lookup"><span data-stu-id="c6d52-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6d52-121">id</span><span class="sxs-lookup"><span data-stu-id="c6d52-121">id</span></span>|<span data-ttu-id="c6d52-122">String</span><span class="sxs-lookup"><span data-stu-id="c6d52-122">String</span></span>|<span data-ttu-id="c6d52-123">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c6d52-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="c6d52-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="c6d52-124">overallScore</span></span>|<span data-ttu-id="c6d52-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c6d52-125">Int32</span></span>|<span data-ttu-id="c6d52-126">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="c6d52-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="c6d52-127">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="c6d52-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="c6d52-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c6d52-128">Int32</span></span>|<span data-ttu-id="c6d52-129">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="c6d52-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="c6d52-130">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="c6d52-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="c6d52-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c6d52-131">Int32</span></span>|<span data-ttu-id="c6d52-132">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="c6d52-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="c6d52-133">insights</span><span class="sxs-lookup"><span data-stu-id="c6d52-133">insights</span></span>|<span data-ttu-id="c6d52-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6d52-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="c6d52-135">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="c6d52-135">The user experience analytics insights.</span></span>|
|<span data-ttu-id="c6d52-136">state</span><span class="sxs-lookup"><span data-stu-id="c6d52-136">state</span></span>|[<span data-ttu-id="c6d52-137">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="c6d52-137">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="c6d52-138">User experience analytics 概述的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="c6d52-138">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="c6d52-139">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="c6d52-139">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="c6d52-140">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="c6d52-140">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="c6d52-141">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="c6d52-141">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="c6d52-142">User experience analytics "BootPerformance" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="c6d52-142">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="c6d52-143">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="c6d52-143">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="c6d52-144">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="c6d52-144">bestPracticesHealthState</span></span>|[<span data-ttu-id="c6d52-145">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="c6d52-145">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="c6d52-146">User experience analytics "BestPractices" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="c6d52-146">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="c6d52-147">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="c6d52-147">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6d52-148">关系</span><span class="sxs-lookup"><span data-stu-id="c6d52-148">Relationships</span></span>
<span data-ttu-id="c6d52-149">无</span><span class="sxs-lookup"><span data-stu-id="c6d52-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6d52-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6d52-150">JSON Representation</span></span>
<span data-ttu-id="c6d52-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6d52-151">Here is a JSON representation of the resource.</span></span>
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



