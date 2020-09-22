---
title: userExperienceAnalyticsCategory 资源类型
description: "\"用户体验分析类别\" 实体包含类别的各个指标的分数和见解。"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eff1c284140b0a4b6b119f073431c13e176b9196
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080934"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="78bf7-103">userExperienceAnalyticsCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="78bf7-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="78bf7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78bf7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78bf7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="78bf7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78bf7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78bf7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78bf7-107">"用户体验分析类别" 实体包含类别的各个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="78bf7-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="78bf7-108">方法</span><span class="sxs-lookup"><span data-stu-id="78bf7-108">Methods</span></span>
|<span data-ttu-id="78bf7-109">方法</span><span class="sxs-lookup"><span data-stu-id="78bf7-109">Method</span></span>|<span data-ttu-id="78bf7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="78bf7-110">Return Type</span></span>|<span data-ttu-id="78bf7-111">说明</span><span class="sxs-lookup"><span data-stu-id="78bf7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78bf7-112">获取 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="78bf7-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="78bf7-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="78bf7-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="78bf7-114">读取 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="78bf7-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="78bf7-115">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="78bf7-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="78bf7-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="78bf7-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="78bf7-117">更新 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="78bf7-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="78bf7-118">属性</span><span class="sxs-lookup"><span data-stu-id="78bf7-118">Properties</span></span>
|<span data-ttu-id="78bf7-119">属性</span><span class="sxs-lookup"><span data-stu-id="78bf7-119">Property</span></span>|<span data-ttu-id="78bf7-120">类型</span><span class="sxs-lookup"><span data-stu-id="78bf7-120">Type</span></span>|<span data-ttu-id="78bf7-121">说明</span><span class="sxs-lookup"><span data-stu-id="78bf7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78bf7-122">id</span><span class="sxs-lookup"><span data-stu-id="78bf7-122">id</span></span>|<span data-ttu-id="78bf7-123">字符串</span><span class="sxs-lookup"><span data-stu-id="78bf7-123">String</span></span>|<span data-ttu-id="78bf7-124">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="78bf7-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="78bf7-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="78bf7-125">overallScore</span></span>|<span data-ttu-id="78bf7-126">Int32</span><span class="sxs-lookup"><span data-stu-id="78bf7-126">Int32</span></span>|<span data-ttu-id="78bf7-127">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="78bf7-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="78bf7-128">insights</span><span class="sxs-lookup"><span data-stu-id="78bf7-128">insights</span></span>|<span data-ttu-id="78bf7-129">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78bf7-129">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="78bf7-130">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="78bf7-130">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="78bf7-131">state</span><span class="sxs-lookup"><span data-stu-id="78bf7-131">state</span></span>|[<span data-ttu-id="78bf7-132">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="78bf7-132">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="78bf7-133">"用户体验分析" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="78bf7-133">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="78bf7-134">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="78bf7-134">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78bf7-135">关系</span><span class="sxs-lookup"><span data-stu-id="78bf7-135">Relationships</span></span>
|<span data-ttu-id="78bf7-136">关系</span><span class="sxs-lookup"><span data-stu-id="78bf7-136">Relationship</span></span>|<span data-ttu-id="78bf7-137">类型</span><span class="sxs-lookup"><span data-stu-id="78bf7-137">Type</span></span>|<span data-ttu-id="78bf7-138">说明</span><span class="sxs-lookup"><span data-stu-id="78bf7-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78bf7-139">metricValues</span><span class="sxs-lookup"><span data-stu-id="78bf7-139">metricValues</span></span>|<span data-ttu-id="78bf7-140">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78bf7-140">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="78bf7-141">User experience analytics 类别的指标值。</span><span class="sxs-lookup"><span data-stu-id="78bf7-141">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78bf7-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78bf7-142">JSON Representation</span></span>
<span data-ttu-id="78bf7-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78bf7-143">Here is a JSON representation of the resource.</span></span>
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
          "value": "4.2"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String"
}
```






