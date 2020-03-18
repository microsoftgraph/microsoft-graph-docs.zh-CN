---
title: userExperienceAnalyticsCategory 资源类型
description: "\"用户体验分析类别\" 实体包含类别的各个指标的分数和见解。"
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ba9d56e1b20b66efe2b0653358dca4907ca0dc2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783835"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="5a0b7-103">userExperienceAnalyticsCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a0b7-103">userExperienceAnalyticsCategory resource type</span></span>

> <span data-ttu-id="5a0b7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a0b7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a0b7-106">"用户体验分析类别" 实体包含类别的各个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-106">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="5a0b7-107">方法</span><span class="sxs-lookup"><span data-stu-id="5a0b7-107">Methods</span></span>
|<span data-ttu-id="5a0b7-108">方法</span><span class="sxs-lookup"><span data-stu-id="5a0b7-108">Method</span></span>|<span data-ttu-id="5a0b7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5a0b7-109">Return Type</span></span>|<span data-ttu-id="5a0b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="5a0b7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a0b7-111">获取 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="5a0b7-111">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="5a0b7-112">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="5a0b7-112">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="5a0b7-113">读取[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-113">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="5a0b7-114">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="5a0b7-114">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="5a0b7-115">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="5a0b7-115">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="5a0b7-116">更新[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-116">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a0b7-117">属性</span><span class="sxs-lookup"><span data-stu-id="5a0b7-117">Properties</span></span>
|<span data-ttu-id="5a0b7-118">属性</span><span class="sxs-lookup"><span data-stu-id="5a0b7-118">Property</span></span>|<span data-ttu-id="5a0b7-119">类型</span><span class="sxs-lookup"><span data-stu-id="5a0b7-119">Type</span></span>|<span data-ttu-id="5a0b7-120">说明</span><span class="sxs-lookup"><span data-stu-id="5a0b7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a0b7-121">id</span><span class="sxs-lookup"><span data-stu-id="5a0b7-121">id</span></span>|<span data-ttu-id="5a0b7-122">String</span><span class="sxs-lookup"><span data-stu-id="5a0b7-122">String</span></span>|<span data-ttu-id="5a0b7-123">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-123">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="5a0b7-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="5a0b7-124">overallScore</span></span>|<span data-ttu-id="5a0b7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="5a0b7-125">Int32</span></span>|<span data-ttu-id="5a0b7-126">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-126">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="5a0b7-127">insights</span><span class="sxs-lookup"><span data-stu-id="5a0b7-127">insights</span></span>|<span data-ttu-id="5a0b7-128">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="5a0b7-128">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="5a0b7-129">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-129">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="5a0b7-130">state</span><span class="sxs-lookup"><span data-stu-id="5a0b7-130">state</span></span>|[<span data-ttu-id="5a0b7-131">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="5a0b7-131">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="5a0b7-132">"用户体验分析" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-132">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="5a0b7-133">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-133">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a0b7-134">关系</span><span class="sxs-lookup"><span data-stu-id="5a0b7-134">Relationships</span></span>
|<span data-ttu-id="5a0b7-135">关系</span><span class="sxs-lookup"><span data-stu-id="5a0b7-135">Relationship</span></span>|<span data-ttu-id="5a0b7-136">类型</span><span class="sxs-lookup"><span data-stu-id="5a0b7-136">Type</span></span>|<span data-ttu-id="5a0b7-137">说明</span><span class="sxs-lookup"><span data-stu-id="5a0b7-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a0b7-138">metricValues</span><span class="sxs-lookup"><span data-stu-id="5a0b7-138">metricValues</span></span>|<span data-ttu-id="5a0b7-139">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)集合</span><span class="sxs-lookup"><span data-stu-id="5a0b7-139">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="5a0b7-140">User experience analytics 类别的指标值。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-140">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a0b7-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a0b7-141">JSON Representation</span></span>
<span data-ttu-id="5a0b7-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a0b7-142">Here is a JSON representation of the resource.</span></span>
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
  "overallScore": 1024,
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



