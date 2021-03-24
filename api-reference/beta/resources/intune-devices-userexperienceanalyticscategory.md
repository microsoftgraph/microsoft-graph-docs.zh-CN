---
title: userExperienceAnalyticsCategory 资源类型
description: 用户体验分析类别实体包含类别的各种指标的分数和见解。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f138b2417bccd6ed089810335e375eb721af80c6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141440"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="ebfac-103">userExperienceAnalyticsCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebfac-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="ebfac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebfac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebfac-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebfac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebfac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebfac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebfac-107">用户体验分析类别实体包含类别的各种指标的分数和见解。</span><span class="sxs-lookup"><span data-stu-id="ebfac-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="ebfac-108">方法</span><span class="sxs-lookup"><span data-stu-id="ebfac-108">Methods</span></span>
|<span data-ttu-id="ebfac-109">方法</span><span class="sxs-lookup"><span data-stu-id="ebfac-109">Method</span></span>|<span data-ttu-id="ebfac-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ebfac-110">Return Type</span></span>|<span data-ttu-id="ebfac-111">说明</span><span class="sxs-lookup"><span data-stu-id="ebfac-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebfac-112">获取 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ebfac-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="ebfac-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ebfac-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="ebfac-114">读取 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebfac-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="ebfac-115">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ebfac-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="ebfac-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ebfac-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="ebfac-117">更新 [userExperienceAnalyticsCategory 对象](../resources/intune-devices-userexperienceanalyticscategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ebfac-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebfac-118">属性</span><span class="sxs-lookup"><span data-stu-id="ebfac-118">Properties</span></span>
|<span data-ttu-id="ebfac-119">属性</span><span class="sxs-lookup"><span data-stu-id="ebfac-119">Property</span></span>|<span data-ttu-id="ebfac-120">类型</span><span class="sxs-lookup"><span data-stu-id="ebfac-120">Type</span></span>|<span data-ttu-id="ebfac-121">说明</span><span class="sxs-lookup"><span data-stu-id="ebfac-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfac-122">id</span><span class="sxs-lookup"><span data-stu-id="ebfac-122">id</span></span>|<span data-ttu-id="ebfac-123">String</span><span class="sxs-lookup"><span data-stu-id="ebfac-123">String</span></span>|<span data-ttu-id="ebfac-124">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ebfac-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="ebfac-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="ebfac-125">overallScore</span></span>|<span data-ttu-id="ebfac-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ebfac-126">Int32</span></span>|<span data-ttu-id="ebfac-127">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="ebfac-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="ebfac-128">totalDevices</span><span class="sxs-lookup"><span data-stu-id="ebfac-128">totalDevices</span></span>|<span data-ttu-id="ebfac-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ebfac-129">Int32</span></span>|<span data-ttu-id="ebfac-130">用户体验分析类别的设备总数。</span><span class="sxs-lookup"><span data-stu-id="ebfac-130">The total device count of the user experience analytics category.</span></span>|
|<span data-ttu-id="ebfac-131">insights</span><span class="sxs-lookup"><span data-stu-id="ebfac-131">insights</span></span>|<span data-ttu-id="ebfac-132">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebfac-132">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="ebfac-133">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="ebfac-133">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="ebfac-134">state</span><span class="sxs-lookup"><span data-stu-id="ebfac-134">state</span></span>|[<span data-ttu-id="ebfac-135">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="ebfac-135">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="ebfac-136">用户体验分析类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="ebfac-136">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="ebfac-137">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="ebfac-137">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebfac-138">关系</span><span class="sxs-lookup"><span data-stu-id="ebfac-138">Relationships</span></span>
|<span data-ttu-id="ebfac-139">关系</span><span class="sxs-lookup"><span data-stu-id="ebfac-139">Relationship</span></span>|<span data-ttu-id="ebfac-140">类型</span><span class="sxs-lookup"><span data-stu-id="ebfac-140">Type</span></span>|<span data-ttu-id="ebfac-141">说明</span><span class="sxs-lookup"><span data-stu-id="ebfac-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfac-142">metricValues</span><span class="sxs-lookup"><span data-stu-id="ebfac-142">metricValues</span></span>|<span data-ttu-id="ebfac-143">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebfac-143">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="ebfac-144">用户体验分析类别的指标值。</span><span class="sxs-lookup"><span data-stu-id="ebfac-144">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebfac-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebfac-145">JSON Representation</span></span>
<span data-ttu-id="ebfac-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebfac-146">Here is a JSON representation of the resource.</span></span>
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
  "totalDevices": 1024,
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




