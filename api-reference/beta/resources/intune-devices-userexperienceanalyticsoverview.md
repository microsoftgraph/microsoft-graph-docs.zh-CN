---
title: userExperienceAnalyticsOverview 资源类型
description: User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 90a33468dfe0d68303625f7a682fdc23d34b7504
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536109"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="69825-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="69825-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="69825-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69825-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69825-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69825-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69825-106">User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="69825-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="69825-107">方法</span><span class="sxs-lookup"><span data-stu-id="69825-107">Methods</span></span>
|<span data-ttu-id="69825-108">方法</span><span class="sxs-lookup"><span data-stu-id="69825-108">Method</span></span>|<span data-ttu-id="69825-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="69825-109">Return Type</span></span>|<span data-ttu-id="69825-110">说明</span><span class="sxs-lookup"><span data-stu-id="69825-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69825-111">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="69825-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="69825-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="69825-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="69825-113">读取[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69825-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="69825-114">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="69825-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="69825-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="69825-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="69825-116">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69825-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69825-117">属性</span><span class="sxs-lookup"><span data-stu-id="69825-117">Properties</span></span>
|<span data-ttu-id="69825-118">属性</span><span class="sxs-lookup"><span data-stu-id="69825-118">Property</span></span>|<span data-ttu-id="69825-119">类型</span><span class="sxs-lookup"><span data-stu-id="69825-119">Type</span></span>|<span data-ttu-id="69825-120">说明</span><span class="sxs-lookup"><span data-stu-id="69825-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69825-121">id</span><span class="sxs-lookup"><span data-stu-id="69825-121">id</span></span>|<span data-ttu-id="69825-122">字符串</span><span class="sxs-lookup"><span data-stu-id="69825-122">String</span></span>|<span data-ttu-id="69825-123">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="69825-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="69825-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="69825-124">overallScore</span></span>|<span data-ttu-id="69825-125">Int32</span><span class="sxs-lookup"><span data-stu-id="69825-125">Int32</span></span>|<span data-ttu-id="69825-126">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="69825-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="69825-127">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="69825-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="69825-128">Int32</span><span class="sxs-lookup"><span data-stu-id="69825-128">Int32</span></span>|<span data-ttu-id="69825-129">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="69825-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="69825-130">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="69825-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="69825-131">Int32</span><span class="sxs-lookup"><span data-stu-id="69825-131">Int32</span></span>|<span data-ttu-id="69825-132">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="69825-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="69825-133">insights</span><span class="sxs-lookup"><span data-stu-id="69825-133">insights</span></span>|<span data-ttu-id="69825-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="69825-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="69825-135">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="69825-135">The user experience analytics insights.</span></span>|
|<span data-ttu-id="69825-136">state</span><span class="sxs-lookup"><span data-stu-id="69825-136">state</span></span>|[<span data-ttu-id="69825-137">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="69825-137">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="69825-138">User experience analytics 概述的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="69825-138">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="69825-139">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="69825-139">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="69825-140">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="69825-140">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="69825-141">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="69825-141">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="69825-142">User experience analytics "BootPerformance" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="69825-142">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="69825-143">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="69825-143">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="69825-144">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="69825-144">bestPracticesHealthState</span></span>|[<span data-ttu-id="69825-145">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="69825-145">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="69825-146">User experience analytics "BestPractices" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="69825-146">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="69825-147">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="69825-147">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69825-148">关系</span><span class="sxs-lookup"><span data-stu-id="69825-148">Relationships</span></span>
<span data-ttu-id="69825-149">无</span><span class="sxs-lookup"><span data-stu-id="69825-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69825-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69825-150">JSON Representation</span></span>
<span data-ttu-id="69825-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69825-151">Here is a JSON representation of the resource.</span></span>
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



