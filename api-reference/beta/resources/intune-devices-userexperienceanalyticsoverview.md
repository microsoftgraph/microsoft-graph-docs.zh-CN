---
title: userExperienceAnalyticsOverview 资源类型
description: User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad7d65e041f8d62e5a8de8aaa9d2f9963b8066b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528452"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="82783-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="82783-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="82783-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="82783-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82783-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82783-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82783-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82783-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82783-107">User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="82783-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="82783-108">方法</span><span class="sxs-lookup"><span data-stu-id="82783-108">Methods</span></span>
|<span data-ttu-id="82783-109">方法</span><span class="sxs-lookup"><span data-stu-id="82783-109">Method</span></span>|<span data-ttu-id="82783-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="82783-110">Return Type</span></span>|<span data-ttu-id="82783-111">说明</span><span class="sxs-lookup"><span data-stu-id="82783-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="82783-112">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="82783-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="82783-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="82783-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="82783-114">读取[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="82783-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="82783-115">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="82783-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="82783-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="82783-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="82783-117">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82783-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="82783-118">属性</span><span class="sxs-lookup"><span data-stu-id="82783-118">Properties</span></span>
|<span data-ttu-id="82783-119">属性</span><span class="sxs-lookup"><span data-stu-id="82783-119">Property</span></span>|<span data-ttu-id="82783-120">类型</span><span class="sxs-lookup"><span data-stu-id="82783-120">Type</span></span>|<span data-ttu-id="82783-121">说明</span><span class="sxs-lookup"><span data-stu-id="82783-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82783-122">id</span><span class="sxs-lookup"><span data-stu-id="82783-122">id</span></span>|<span data-ttu-id="82783-123">String</span><span class="sxs-lookup"><span data-stu-id="82783-123">String</span></span>|<span data-ttu-id="82783-124">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="82783-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="82783-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="82783-125">overallScore</span></span>|<span data-ttu-id="82783-126">Int32</span><span class="sxs-lookup"><span data-stu-id="82783-126">Int32</span></span>|<span data-ttu-id="82783-127">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="82783-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="82783-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="82783-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="82783-129">Int32</span><span class="sxs-lookup"><span data-stu-id="82783-129">Int32</span></span>|<span data-ttu-id="82783-130">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="82783-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="82783-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="82783-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="82783-132">Int32</span><span class="sxs-lookup"><span data-stu-id="82783-132">Int32</span></span>|<span data-ttu-id="82783-133">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="82783-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="82783-134">insights</span><span class="sxs-lookup"><span data-stu-id="82783-134">insights</span></span>|<span data-ttu-id="82783-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="82783-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="82783-136">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="82783-136">The user experience analytics insights.</span></span>|
|<span data-ttu-id="82783-137">state</span><span class="sxs-lookup"><span data-stu-id="82783-137">state</span></span>|[<span data-ttu-id="82783-138">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="82783-138">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="82783-139">User experience analytics 概述的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="82783-139">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="82783-140">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="82783-140">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="82783-141">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="82783-141">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="82783-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="82783-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="82783-143">User experience analytics "BootPerformance" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="82783-143">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="82783-144">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="82783-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="82783-145">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="82783-145">bestPracticesHealthState</span></span>|[<span data-ttu-id="82783-146">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="82783-146">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="82783-147">User experience analytics "BestPractices" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="82783-147">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="82783-148">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="82783-148">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82783-149">关系</span><span class="sxs-lookup"><span data-stu-id="82783-149">Relationships</span></span>
<span data-ttu-id="82783-150">无</span><span class="sxs-lookup"><span data-stu-id="82783-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82783-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82783-151">JSON Representation</span></span>
<span data-ttu-id="82783-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82783-152">Here is a JSON representation of the resource.</span></span>
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



