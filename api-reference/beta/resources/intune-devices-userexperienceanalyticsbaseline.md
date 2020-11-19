---
title: userExperienceAnalyticsBaseline 资源类型
description: User experience analytics 基线实体包含比较用户体验分析得分所依据的基线值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e48064e7cc5f0d3a0901dd6b6ff320224403a9c3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208441"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a><span data-ttu-id="cf2ba-103">userExperienceAnalyticsBaseline 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf2ba-103">userExperienceAnalyticsBaseline resource type</span></span>

<span data-ttu-id="cf2ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf2ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf2ba-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf2ba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf2ba-107">User experience analytics 基线实体包含比较用户体验分析得分所依据的基线值。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-107">The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores.</span></span>

## <a name="methods"></a><span data-ttu-id="cf2ba-108">方法</span><span class="sxs-lookup"><span data-stu-id="cf2ba-108">Methods</span></span>
|<span data-ttu-id="cf2ba-109">方法</span><span class="sxs-lookup"><span data-stu-id="cf2ba-109">Method</span></span>|<span data-ttu-id="cf2ba-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf2ba-110">Return Type</span></span>|<span data-ttu-id="cf2ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="cf2ba-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf2ba-112">列出 userExperienceAnalyticsBaselines</span><span class="sxs-lookup"><span data-stu-id="cf2ba-112">List userExperienceAnalyticsBaselines</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|<span data-ttu-id="cf2ba-113">[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cf2ba-113">[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) collection</span></span>|<span data-ttu-id="cf2ba-114">列出 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-114">List properties and relationships of the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) objects.</span></span>|
|[<span data-ttu-id="cf2ba-115">获取 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="cf2ba-115">Get userExperienceAnalyticsBaseline</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[<span data-ttu-id="cf2ba-116">userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="cf2ba-116">userExperienceAnalyticsBaseline</span></span>](../resources/intune-devices-userexperienceanalyticsbaseline.md)|<span data-ttu-id="cf2ba-117">读取 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-117">Read properties and relationships of the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>|
|[<span data-ttu-id="cf2ba-118">创建 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="cf2ba-118">Create userExperienceAnalyticsBaseline</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[<span data-ttu-id="cf2ba-119">userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="cf2ba-119">userExperienceAnalyticsBaseline</span></span>](../resources/intune-devices-userexperienceanalyticsbaseline.md)|<span data-ttu-id="cf2ba-120">创建新的 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-120">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>|
|[<span data-ttu-id="cf2ba-121">删除 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="cf2ba-121">Delete userExperienceAnalyticsBaseline</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|<span data-ttu-id="cf2ba-122">无</span><span class="sxs-lookup"><span data-stu-id="cf2ba-122">None</span></span>|<span data-ttu-id="cf2ba-123">删除 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-123">Deletes a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>|
|[<span data-ttu-id="cf2ba-124">更新 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="cf2ba-124">Update userExperienceAnalyticsBaseline</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[<span data-ttu-id="cf2ba-125">userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="cf2ba-125">userExperienceAnalyticsBaseline</span></span>](../resources/intune-devices-userexperienceanalyticsbaseline.md)|<span data-ttu-id="cf2ba-126">更新 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-126">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf2ba-127">属性</span><span class="sxs-lookup"><span data-stu-id="cf2ba-127">Properties</span></span>
|<span data-ttu-id="cf2ba-128">属性</span><span class="sxs-lookup"><span data-stu-id="cf2ba-128">Property</span></span>|<span data-ttu-id="cf2ba-129">类型</span><span class="sxs-lookup"><span data-stu-id="cf2ba-129">Type</span></span>|<span data-ttu-id="cf2ba-130">说明</span><span class="sxs-lookup"><span data-stu-id="cf2ba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf2ba-131">id</span><span class="sxs-lookup"><span data-stu-id="cf2ba-131">id</span></span>|<span data-ttu-id="cf2ba-132">String</span><span class="sxs-lookup"><span data-stu-id="cf2ba-132">String</span></span>|<span data-ttu-id="cf2ba-133">User experience analytics 比较基准的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-133">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="cf2ba-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cf2ba-134">displayName</span></span>|<span data-ttu-id="cf2ba-135">String</span><span class="sxs-lookup"><span data-stu-id="cf2ba-135">String</span></span>|<span data-ttu-id="cf2ba-136">User experience analytics 基线的名称。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-136">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="cf2ba-137">overallScore</span><span class="sxs-lookup"><span data-stu-id="cf2ba-137">overallScore</span></span>|<span data-ttu-id="cf2ba-138">Int32</span><span class="sxs-lookup"><span data-stu-id="cf2ba-138">Int32</span></span>|<span data-ttu-id="cf2ba-139">用户体验分析基准的总体分数。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-139">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="cf2ba-140">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cf2ba-140">isBuiltIn</span></span>|<span data-ttu-id="cf2ba-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2ba-141">Boolean</span></span>|<span data-ttu-id="cf2ba-142">指示当前基线是商业中间基线还是自定义基线。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-142">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="cf2ba-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf2ba-143">createdDateTime</span></span>|<span data-ttu-id="cf2ba-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf2ba-144">DateTimeOffset</span></span>|<span data-ttu-id="cf2ba-145">自定义基线的创建日期。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-145">The date the custom baseline was created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf2ba-146">关系</span><span class="sxs-lookup"><span data-stu-id="cf2ba-146">Relationships</span></span>
|<span data-ttu-id="cf2ba-147">关系</span><span class="sxs-lookup"><span data-stu-id="cf2ba-147">Relationship</span></span>|<span data-ttu-id="cf2ba-148">类型</span><span class="sxs-lookup"><span data-stu-id="cf2ba-148">Type</span></span>|<span data-ttu-id="cf2ba-149">说明</span><span class="sxs-lookup"><span data-stu-id="cf2ba-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf2ba-150">deviceBootPerformanceMetrics</span><span class="sxs-lookup"><span data-stu-id="cf2ba-150">deviceBootPerformanceMetrics</span></span>|[<span data-ttu-id="cf2ba-151">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cf2ba-151">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="cf2ba-152">User experience analytics 设备启动性能指标。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-152">The user experience analytics device boot performance metrics.</span></span>|
|<span data-ttu-id="cf2ba-153">bestPracticesMetrics</span><span class="sxs-lookup"><span data-stu-id="cf2ba-153">bestPracticesMetrics</span></span>|[<span data-ttu-id="cf2ba-154">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cf2ba-154">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="cf2ba-155">用户体验分析最佳实践指标。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-155">The user experience analytics best practices metrics.</span></span>|
|<span data-ttu-id="cf2ba-156">rebootAnalyticsMetrics</span><span class="sxs-lookup"><span data-stu-id="cf2ba-156">rebootAnalyticsMetrics</span></span>|[<span data-ttu-id="cf2ba-157">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cf2ba-157">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="cf2ba-158">用户体验分析重新启动分析指标。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-158">The user experience analytics reboot analytics metrics.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf2ba-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf2ba-159">JSON Representation</span></span>
<span data-ttu-id="cf2ba-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf2ba-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "isBuiltIn": true,
  "createdDateTime": "String (timestamp)"
}
```




