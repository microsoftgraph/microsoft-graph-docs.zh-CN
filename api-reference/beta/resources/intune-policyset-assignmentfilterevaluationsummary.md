---
title: assignmentFilterEvaluationSummary 资源类型
description: 表示工作分配筛选器评估的结果摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05c9a3eabd22e7e22a6d74229b7aa47901e05db6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155979"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a><span data-ttu-id="6bacc-103">assignmentFilterEvaluationSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bacc-103">assignmentFilterEvaluationSummary resource type</span></span>

<span data-ttu-id="6bacc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bacc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bacc-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6bacc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bacc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6bacc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bacc-107">表示工作分配筛选器评估的结果摘要</span><span class="sxs-lookup"><span data-stu-id="6bacc-107">Represent result summary for assignment filter evaluation</span></span>

## <a name="properties"></a><span data-ttu-id="6bacc-108">属性</span><span class="sxs-lookup"><span data-stu-id="6bacc-108">Properties</span></span>
|<span data-ttu-id="6bacc-109">属性</span><span class="sxs-lookup"><span data-stu-id="6bacc-109">Property</span></span>|<span data-ttu-id="6bacc-110">类型</span><span class="sxs-lookup"><span data-stu-id="6bacc-110">Type</span></span>|<span data-ttu-id="6bacc-111">说明</span><span class="sxs-lookup"><span data-stu-id="6bacc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bacc-112">assignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="6bacc-112">assignmentFilterId</span></span>|<span data-ttu-id="6bacc-113">String</span><span class="sxs-lookup"><span data-stu-id="6bacc-113">String</span></span>|<span data-ttu-id="6bacc-114">分配筛选器对象的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="6bacc-114">Unique identifier for the assignment filter object</span></span>|
|<span data-ttu-id="6bacc-115">assignmentFilterLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bacc-115">assignmentFilterLastModifiedDateTime</span></span>|<span data-ttu-id="6bacc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bacc-116">DateTimeOffset</span></span>|<span data-ttu-id="6bacc-117">上次修改工作分配筛选器的时间。</span><span class="sxs-lookup"><span data-stu-id="6bacc-117">The time the assignment filter was last modified.</span></span>|
|<span data-ttu-id="6bacc-118">assignmentFilterDisplayName</span><span class="sxs-lookup"><span data-stu-id="6bacc-118">assignmentFilterDisplayName</span></span>|<span data-ttu-id="6bacc-119">String</span><span class="sxs-lookup"><span data-stu-id="6bacc-119">String</span></span>|<span data-ttu-id="6bacc-120">管理员为分配筛选器定义的名称。</span><span class="sxs-lookup"><span data-stu-id="6bacc-120">The admin defined name for assignment filter.</span></span>|
|<span data-ttu-id="6bacc-121">assignmentFilterPlatform</span><span class="sxs-lookup"><span data-stu-id="6bacc-121">assignmentFilterPlatform</span></span>|[<span data-ttu-id="6bacc-122">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="6bacc-122">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="6bacc-123">创建此分配筛选器的平台。</span><span class="sxs-lookup"><span data-stu-id="6bacc-123">The platform for which this assignment filter is created.</span></span> <span data-ttu-id="6bacc-124">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="6bacc-124">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="6bacc-125">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="6bacc-125">evaluationResult</span></span>|[<span data-ttu-id="6bacc-126">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="6bacc-126">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="6bacc-127">工作分配筛选器评估结果。</span><span class="sxs-lookup"><span data-stu-id="6bacc-127">Assignment filter evaluation result.</span></span> <span data-ttu-id="6bacc-128">可取值为：`unknown`、`match`、`notMatch`、`inconclusive`、`failure`、`notEvaluated`。</span><span class="sxs-lookup"><span data-stu-id="6bacc-128">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|
|<span data-ttu-id="6bacc-129">evaluationDateTime</span><span class="sxs-lookup"><span data-stu-id="6bacc-129">evaluationDateTime</span></span>|<span data-ttu-id="6bacc-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bacc-130">DateTimeOffset</span></span>|<span data-ttu-id="6bacc-131">已评估时间分配筛选器。</span><span class="sxs-lookup"><span data-stu-id="6bacc-131">The time assignment filter was evaluated.</span></span>|
|<span data-ttu-id="6bacc-132">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6bacc-132">assignmentFilterType</span></span>|[<span data-ttu-id="6bacc-133">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6bacc-133">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="6bacc-134">指示包含或排除筛选器类型。</span><span class="sxs-lookup"><span data-stu-id="6bacc-134">Indicate filter type either include or exclude.</span></span> <span data-ttu-id="6bacc-135">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="6bacc-135">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="6bacc-136">assignmentFilterTypeAndEvaluationResults</span><span class="sxs-lookup"><span data-stu-id="6bacc-136">assignmentFilterTypeAndEvaluationResults</span></span>|<span data-ttu-id="6bacc-137">[assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bacc-137">[assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md) collection</span></span>|<span data-ttu-id="6bacc-138">筛选器类型及其相应的评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="6bacc-138">A collection of filter types and their corresponding evaluation results.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bacc-139">关系</span><span class="sxs-lookup"><span data-stu-id="6bacc-139">Relationships</span></span>
<span data-ttu-id="6bacc-140">无</span><span class="sxs-lookup"><span data-stu-id="6bacc-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bacc-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bacc-141">JSON Representation</span></span>
<span data-ttu-id="6bacc-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bacc-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationSummary",
  "assignmentFilterId": "String",
  "assignmentFilterLastModifiedDateTime": "String (timestamp)",
  "assignmentFilterDisplayName": "String",
  "assignmentFilterPlatform": "String",
  "evaluationResult": "String",
  "evaluationDateTime": "String (timestamp)",
  "assignmentFilterType": "String",
  "assignmentFilterTypeAndEvaluationResults": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
      "assignmentFilterType": "String",
      "evaluationResult": "String"
    }
  ]
}
```




