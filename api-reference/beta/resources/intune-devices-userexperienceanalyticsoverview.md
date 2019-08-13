---
title: userExperienceAnalyticsOverview 资源类型
description: User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff3be73059f913943236bfce8bcb4e729a39081d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371458"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="fcaf0-103">userExperienceAnalyticsOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcaf0-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="fcaf0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcaf0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcaf0-106">User experience analytics 概述实体包含所有类别的总分数和每个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="fcaf0-107">方法</span><span class="sxs-lookup"><span data-stu-id="fcaf0-107">Methods</span></span>
|<span data-ttu-id="fcaf0-108">方法</span><span class="sxs-lookup"><span data-stu-id="fcaf0-108">Method</span></span>|<span data-ttu-id="fcaf0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fcaf0-109">Return Type</span></span>|<span data-ttu-id="fcaf0-110">说明</span><span class="sxs-lookup"><span data-stu-id="fcaf0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fcaf0-111">获取 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="fcaf0-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="fcaf0-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="fcaf0-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="fcaf0-113">读取[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="fcaf0-114">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="fcaf0-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="fcaf0-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="fcaf0-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="fcaf0-116">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fcaf0-117">属性</span><span class="sxs-lookup"><span data-stu-id="fcaf0-117">Properties</span></span>
|<span data-ttu-id="fcaf0-118">属性</span><span class="sxs-lookup"><span data-stu-id="fcaf0-118">Property</span></span>|<span data-ttu-id="fcaf0-119">类型</span><span class="sxs-lookup"><span data-stu-id="fcaf0-119">Type</span></span>|<span data-ttu-id="fcaf0-120">说明</span><span class="sxs-lookup"><span data-stu-id="fcaf0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcaf0-121">id</span><span class="sxs-lookup"><span data-stu-id="fcaf0-121">id</span></span>|<span data-ttu-id="fcaf0-122">String</span><span class="sxs-lookup"><span data-stu-id="fcaf0-122">String</span></span>|<span data-ttu-id="fcaf0-123">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="fcaf0-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="fcaf0-124">overallScore</span></span>|<span data-ttu-id="fcaf0-125">Int32</span><span class="sxs-lookup"><span data-stu-id="fcaf0-125">Int32</span></span>|<span data-ttu-id="fcaf0-126">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="fcaf0-127">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="fcaf0-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="fcaf0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="fcaf0-128">Int32</span></span>|<span data-ttu-id="fcaf0-129">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="fcaf0-130">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="fcaf0-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="fcaf0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="fcaf0-131">Int32</span></span>|<span data-ttu-id="fcaf0-132">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="fcaf0-133">insights</span><span class="sxs-lookup"><span data-stu-id="fcaf0-133">insights</span></span>|<span data-ttu-id="fcaf0-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="fcaf0-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="fcaf0-135">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-135">The user experience analytics insights.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcaf0-136">关系</span><span class="sxs-lookup"><span data-stu-id="fcaf0-136">Relationships</span></span>
<span data-ttu-id="fcaf0-137">无</span><span class="sxs-lookup"><span data-stu-id="fcaf0-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcaf0-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcaf0-138">JSON Representation</span></span>
<span data-ttu-id="fcaf0-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcaf0-139">Here is a JSON representation of the resource.</span></span>
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
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```



