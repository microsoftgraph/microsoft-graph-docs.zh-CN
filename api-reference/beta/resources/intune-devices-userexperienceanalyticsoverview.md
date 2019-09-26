---
title: userExperienceAnalyticsOverview 资源类型
description: User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11c7bbe64b1495a9e6cb0b8ac144d1afb539789f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196670"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="a00dc-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="a00dc-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="a00dc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a00dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a00dc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a00dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a00dc-106">User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="a00dc-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="a00dc-107">方法</span><span class="sxs-lookup"><span data-stu-id="a00dc-107">Methods</span></span>
|<span data-ttu-id="a00dc-108">方法</span><span class="sxs-lookup"><span data-stu-id="a00dc-108">Method</span></span>|<span data-ttu-id="a00dc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a00dc-109">Return Type</span></span>|<span data-ttu-id="a00dc-110">说明</span><span class="sxs-lookup"><span data-stu-id="a00dc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a00dc-111">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a00dc-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="a00dc-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a00dc-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="a00dc-113">读取[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a00dc-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="a00dc-114">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a00dc-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="a00dc-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a00dc-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="a00dc-116">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a00dc-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a00dc-117">属性</span><span class="sxs-lookup"><span data-stu-id="a00dc-117">Properties</span></span>
|<span data-ttu-id="a00dc-118">属性</span><span class="sxs-lookup"><span data-stu-id="a00dc-118">Property</span></span>|<span data-ttu-id="a00dc-119">类型</span><span class="sxs-lookup"><span data-stu-id="a00dc-119">Type</span></span>|<span data-ttu-id="a00dc-120">说明</span><span class="sxs-lookup"><span data-stu-id="a00dc-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a00dc-121">id</span><span class="sxs-lookup"><span data-stu-id="a00dc-121">id</span></span>|<span data-ttu-id="a00dc-122">String</span><span class="sxs-lookup"><span data-stu-id="a00dc-122">String</span></span>|<span data-ttu-id="a00dc-123">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a00dc-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="a00dc-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="a00dc-124">overallScore</span></span>|<span data-ttu-id="a00dc-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a00dc-125">Int32</span></span>|<span data-ttu-id="a00dc-126">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="a00dc-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="a00dc-127">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="a00dc-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="a00dc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a00dc-128">Int32</span></span>|<span data-ttu-id="a00dc-129">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="a00dc-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="a00dc-130">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="a00dc-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="a00dc-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a00dc-131">Int32</span></span>|<span data-ttu-id="a00dc-132">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="a00dc-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="a00dc-133">insights</span><span class="sxs-lookup"><span data-stu-id="a00dc-133">insights</span></span>|<span data-ttu-id="a00dc-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="a00dc-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="a00dc-135">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="a00dc-135">The user experience analytics insights.</span></span>|
|<span data-ttu-id="a00dc-136">state</span><span class="sxs-lookup"><span data-stu-id="a00dc-136">state</span></span>|[<span data-ttu-id="a00dc-137">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a00dc-137">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a00dc-138">"用户体验分析" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="a00dc-138">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="a00dc-139">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="a00dc-139">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a00dc-140">关系</span><span class="sxs-lookup"><span data-stu-id="a00dc-140">Relationships</span></span>
<span data-ttu-id="a00dc-141">无</span><span class="sxs-lookup"><span data-stu-id="a00dc-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a00dc-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a00dc-142">JSON Representation</span></span>
<span data-ttu-id="a00dc-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a00dc-143">Here is a JSON representation of the resource.</span></span>
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
  "state": "String"
}
```



