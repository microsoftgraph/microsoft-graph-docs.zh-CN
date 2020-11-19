---
title: userExperienceAnalyticsCategory 资源类型
description: "\"用户体验分析类别\" 实体包含类别的各个指标的分数和见解。"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fabbc284745969c34a4495a7164007577c45750
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208448"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="01d4a-103">userExperienceAnalyticsCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="01d4a-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="01d4a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01d4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01d4a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01d4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01d4a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01d4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01d4a-107">"用户体验分析类别" 实体包含类别的各个指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="01d4a-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="01d4a-108">方法</span><span class="sxs-lookup"><span data-stu-id="01d4a-108">Methods</span></span>
|<span data-ttu-id="01d4a-109">方法</span><span class="sxs-lookup"><span data-stu-id="01d4a-109">Method</span></span>|<span data-ttu-id="01d4a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="01d4a-110">Return Type</span></span>|<span data-ttu-id="01d4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="01d4a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="01d4a-112">获取 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="01d4a-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="01d4a-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="01d4a-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="01d4a-114">读取 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="01d4a-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="01d4a-115">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="01d4a-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="01d4a-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="01d4a-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="01d4a-117">更新 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="01d4a-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="01d4a-118">属性</span><span class="sxs-lookup"><span data-stu-id="01d4a-118">Properties</span></span>
|<span data-ttu-id="01d4a-119">属性</span><span class="sxs-lookup"><span data-stu-id="01d4a-119">Property</span></span>|<span data-ttu-id="01d4a-120">类型</span><span class="sxs-lookup"><span data-stu-id="01d4a-120">Type</span></span>|<span data-ttu-id="01d4a-121">说明</span><span class="sxs-lookup"><span data-stu-id="01d4a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d4a-122">id</span><span class="sxs-lookup"><span data-stu-id="01d4a-122">id</span></span>|<span data-ttu-id="01d4a-123">String</span><span class="sxs-lookup"><span data-stu-id="01d4a-123">String</span></span>|<span data-ttu-id="01d4a-124">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="01d4a-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="01d4a-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="01d4a-125">overallScore</span></span>|<span data-ttu-id="01d4a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="01d4a-126">Int32</span></span>|<span data-ttu-id="01d4a-127">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="01d4a-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="01d4a-128">insights</span><span class="sxs-lookup"><span data-stu-id="01d4a-128">insights</span></span>|<span data-ttu-id="01d4a-129">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01d4a-129">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="01d4a-130">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="01d4a-130">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="01d4a-131">state</span><span class="sxs-lookup"><span data-stu-id="01d4a-131">state</span></span>|[<span data-ttu-id="01d4a-132">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="01d4a-132">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="01d4a-133">"用户体验分析" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="01d4a-133">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="01d4a-134">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="01d4a-134">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01d4a-135">关系</span><span class="sxs-lookup"><span data-stu-id="01d4a-135">Relationships</span></span>
|<span data-ttu-id="01d4a-136">关系</span><span class="sxs-lookup"><span data-stu-id="01d4a-136">Relationship</span></span>|<span data-ttu-id="01d4a-137">类型</span><span class="sxs-lookup"><span data-stu-id="01d4a-137">Type</span></span>|<span data-ttu-id="01d4a-138">说明</span><span class="sxs-lookup"><span data-stu-id="01d4a-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d4a-139">metricValues</span><span class="sxs-lookup"><span data-stu-id="01d4a-139">metricValues</span></span>|<span data-ttu-id="01d4a-140">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01d4a-140">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="01d4a-141">User experience analytics 类别的指标值。</span><span class="sxs-lookup"><span data-stu-id="01d4a-141">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01d4a-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01d4a-142">JSON Representation</span></span>
<span data-ttu-id="01d4a-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01d4a-143">Here is a JSON representation of the resource.</span></span>
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




