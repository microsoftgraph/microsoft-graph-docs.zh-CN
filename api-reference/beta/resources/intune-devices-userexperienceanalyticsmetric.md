---
title: userExperienceAnalyticsMetric 资源类型
description: User experience analytics 指标包含 user experience anlaytics 类别的分数和度量单位。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e03dbe489f7236358f90dcb305d6328d5017018b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736140"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a><span data-ttu-id="3377f-103">userExperienceAnalyticsMetric 资源类型</span><span class="sxs-lookup"><span data-stu-id="3377f-103">userExperienceAnalyticsMetric resource type</span></span>

<span data-ttu-id="3377f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3377f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3377f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3377f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3377f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3377f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3377f-107">User experience analytics 指标包含 user experience anlaytics 类别的分数和度量单位。</span><span class="sxs-lookup"><span data-stu-id="3377f-107">The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category.</span></span>

## <a name="methods"></a><span data-ttu-id="3377f-108">Methods</span><span class="sxs-lookup"><span data-stu-id="3377f-108">Methods</span></span>
|<span data-ttu-id="3377f-109">方法</span><span class="sxs-lookup"><span data-stu-id="3377f-109">Method</span></span>|<span data-ttu-id="3377f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3377f-110">Return Type</span></span>|<span data-ttu-id="3377f-111">说明</span><span class="sxs-lookup"><span data-stu-id="3377f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3377f-112">列出 userExperienceAnalyticsMetrics</span><span class="sxs-lookup"><span data-stu-id="3377f-112">List userExperienceAnalyticsMetrics</span></span>](../api/intune-devices-userexperienceanalyticsmetric-list.md)|<span data-ttu-id="3377f-113">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3377f-113">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="3377f-114">列出 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3377f-114">List properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects.</span></span>|
|[<span data-ttu-id="3377f-115">获取 userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="3377f-115">Get userExperienceAnalyticsMetric</span></span>](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[<span data-ttu-id="3377f-116">userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="3377f-116">userExperienceAnalyticsMetric</span></span>](../resources/intune-devices-userexperienceanalyticsmetric.md)|<span data-ttu-id="3377f-117">读取 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3377f-117">Read properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>|
|[<span data-ttu-id="3377f-118">创建 userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="3377f-118">Create userExperienceAnalyticsMetric</span></span>](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[<span data-ttu-id="3377f-119">userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="3377f-119">userExperienceAnalyticsMetric</span></span>](../resources/intune-devices-userexperienceanalyticsmetric.md)|<span data-ttu-id="3377f-120">创建新的 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3377f-120">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>|
|[<span data-ttu-id="3377f-121">删除 userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="3377f-121">Delete userExperienceAnalyticsMetric</span></span>](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|<span data-ttu-id="3377f-122">无</span><span class="sxs-lookup"><span data-stu-id="3377f-122">None</span></span>|<span data-ttu-id="3377f-123">删除 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)。</span><span class="sxs-lookup"><span data-stu-id="3377f-123">Deletes a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>|
|[<span data-ttu-id="3377f-124">更新 userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="3377f-124">Update userExperienceAnalyticsMetric</span></span>](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[<span data-ttu-id="3377f-125">userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="3377f-125">userExperienceAnalyticsMetric</span></span>](../resources/intune-devices-userexperienceanalyticsmetric.md)|<span data-ttu-id="3377f-126">更新 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3377f-126">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3377f-127">属性</span><span class="sxs-lookup"><span data-stu-id="3377f-127">Properties</span></span>
|<span data-ttu-id="3377f-128">属性</span><span class="sxs-lookup"><span data-stu-id="3377f-128">Property</span></span>|<span data-ttu-id="3377f-129">类型</span><span class="sxs-lookup"><span data-stu-id="3377f-129">Type</span></span>|<span data-ttu-id="3377f-130">说明</span><span class="sxs-lookup"><span data-stu-id="3377f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3377f-131">id</span><span class="sxs-lookup"><span data-stu-id="3377f-131">id</span></span>|<span data-ttu-id="3377f-132">String</span><span class="sxs-lookup"><span data-stu-id="3377f-132">String</span></span>|<span data-ttu-id="3377f-133">User experience analytics 指标的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3377f-133">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="3377f-134">值</span><span class="sxs-lookup"><span data-stu-id="3377f-134">value</span></span>|<span data-ttu-id="3377f-135">双精度</span><span class="sxs-lookup"><span data-stu-id="3377f-135">Double</span></span>|<span data-ttu-id="3377f-136">User experience analytics 指标的值。</span><span class="sxs-lookup"><span data-stu-id="3377f-136">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="3377f-137">处理器</span><span class="sxs-lookup"><span data-stu-id="3377f-137">unit</span></span>|<span data-ttu-id="3377f-138">String</span><span class="sxs-lookup"><span data-stu-id="3377f-138">String</span></span>|<span data-ttu-id="3377f-139">User experience analytics 指标的单位。</span><span class="sxs-lookup"><span data-stu-id="3377f-139">The unit of the user experience analytics metric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3377f-140">关系</span><span class="sxs-lookup"><span data-stu-id="3377f-140">Relationships</span></span>
<span data-ttu-id="3377f-141">无</span><span class="sxs-lookup"><span data-stu-id="3377f-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3377f-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3377f-142">JSON Representation</span></span>
<span data-ttu-id="3377f-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3377f-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "String (identifier)",
  "value": "4.2",
  "unit": "String"
}
```





