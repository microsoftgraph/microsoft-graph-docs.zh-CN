---
title: userExperienceAnalyticsCategory 资源类型
description: "\"用户体验分析类别\" 实体包含类别的各个指标的分数和见解。"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c04f2caaa7b9ee6c093a58e4c8123250113b3a9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329641"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="30f95-103">userExperienceAnalyticsCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="30f95-103">userExperienceAnalyticsCategory resource type</span></span>

> <span data-ttu-id="30f95-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="30f95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30f95-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="30f95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30f95-106">"用户体验分析类别" 实体包含类别的各个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="30f95-106">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="30f95-107">方法</span><span class="sxs-lookup"><span data-stu-id="30f95-107">Methods</span></span>
|<span data-ttu-id="30f95-108">方法</span><span class="sxs-lookup"><span data-stu-id="30f95-108">Method</span></span>|<span data-ttu-id="30f95-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="30f95-109">Return Type</span></span>|<span data-ttu-id="30f95-110">说明</span><span class="sxs-lookup"><span data-stu-id="30f95-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30f95-111">获取 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="30f95-111">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="30f95-112">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="30f95-112">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="30f95-113">读取[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30f95-113">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="30f95-114">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="30f95-114">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="30f95-115">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="30f95-115">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="30f95-116">更新[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="30f95-116">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30f95-117">属性</span><span class="sxs-lookup"><span data-stu-id="30f95-117">Properties</span></span>
|<span data-ttu-id="30f95-118">属性</span><span class="sxs-lookup"><span data-stu-id="30f95-118">Property</span></span>|<span data-ttu-id="30f95-119">类型</span><span class="sxs-lookup"><span data-stu-id="30f95-119">Type</span></span>|<span data-ttu-id="30f95-120">说明</span><span class="sxs-lookup"><span data-stu-id="30f95-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f95-121">id</span><span class="sxs-lookup"><span data-stu-id="30f95-121">id</span></span>|<span data-ttu-id="30f95-122">String</span><span class="sxs-lookup"><span data-stu-id="30f95-122">String</span></span>|<span data-ttu-id="30f95-123">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="30f95-123">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="30f95-124">displayName</span><span class="sxs-lookup"><span data-stu-id="30f95-124">displayName</span></span>|<span data-ttu-id="30f95-125">String</span><span class="sxs-lookup"><span data-stu-id="30f95-125">String</span></span>|<span data-ttu-id="30f95-126">用户体验分析类别的名称。</span><span class="sxs-lookup"><span data-stu-id="30f95-126">The name of the user experience analytics category.</span></span>|
|<span data-ttu-id="30f95-127">overallScore</span><span class="sxs-lookup"><span data-stu-id="30f95-127">overallScore</span></span>|<span data-ttu-id="30f95-128">Int32</span><span class="sxs-lookup"><span data-stu-id="30f95-128">Int32</span></span>|<span data-ttu-id="30f95-129">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="30f95-129">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="30f95-130">insights</span><span class="sxs-lookup"><span data-stu-id="30f95-130">insights</span></span>|<span data-ttu-id="30f95-131">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="30f95-131">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="30f95-132">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="30f95-132">The insights for the user experience analytics category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30f95-133">关系</span><span class="sxs-lookup"><span data-stu-id="30f95-133">Relationships</span></span>
|<span data-ttu-id="30f95-134">关系</span><span class="sxs-lookup"><span data-stu-id="30f95-134">Relationship</span></span>|<span data-ttu-id="30f95-135">类型</span><span class="sxs-lookup"><span data-stu-id="30f95-135">Type</span></span>|<span data-ttu-id="30f95-136">说明</span><span class="sxs-lookup"><span data-stu-id="30f95-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f95-137">metricValues</span><span class="sxs-lookup"><span data-stu-id="30f95-137">metricValues</span></span>|<span data-ttu-id="30f95-138">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)集合</span><span class="sxs-lookup"><span data-stu-id="30f95-138">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="30f95-139">User experience analytics 类别的指标值。</span><span class="sxs-lookup"><span data-stu-id="30f95-139">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30f95-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30f95-140">JSON Representation</span></span>
<span data-ttu-id="30f95-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30f95-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
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



