---
title: assignmentFilterEvaluationSummary 资源类型
description: 表示工作分配筛选器评估的结果摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31f2e93f481f0b21689b1a83d63f4540c22f50cb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160287"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a><span data-ttu-id="2fa2e-103">assignmentFilterEvaluationSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fa2e-103">assignmentFilterEvaluationSummary resource type</span></span>

<span data-ttu-id="2fa2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fa2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fa2e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fa2e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fa2e-107">表示工作分配筛选器评估的结果摘要</span><span class="sxs-lookup"><span data-stu-id="2fa2e-107">Represent result summary for assignment filter evaluation</span></span>

## <a name="properties"></a><span data-ttu-id="2fa2e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2fa2e-108">Properties</span></span>
|<span data-ttu-id="2fa2e-109">属性</span><span class="sxs-lookup"><span data-stu-id="2fa2e-109">Property</span></span>|<span data-ttu-id="2fa2e-110">类型</span><span class="sxs-lookup"><span data-stu-id="2fa2e-110">Type</span></span>|<span data-ttu-id="2fa2e-111">说明</span><span class="sxs-lookup"><span data-stu-id="2fa2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa2e-112">assignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="2fa2e-112">assignmentFilterId</span></span>|<span data-ttu-id="2fa2e-113">String</span><span class="sxs-lookup"><span data-stu-id="2fa2e-113">String</span></span>|<span data-ttu-id="2fa2e-114">分配筛选器对象的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="2fa2e-114">Unique identifier for the assignment filter object</span></span>|
|<span data-ttu-id="2fa2e-115">assignmentFilterLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa2e-115">assignmentFilterLastModifiedDateTime</span></span>|<span data-ttu-id="2fa2e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa2e-116">DateTimeOffset</span></span>|<span data-ttu-id="2fa2e-117">上次修改工作分配筛选器的时间。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-117">The time the assignment filter was last modified.</span></span>|
|<span data-ttu-id="2fa2e-118">assignmentFilterDisplayName</span><span class="sxs-lookup"><span data-stu-id="2fa2e-118">assignmentFilterDisplayName</span></span>|<span data-ttu-id="2fa2e-119">String</span><span class="sxs-lookup"><span data-stu-id="2fa2e-119">String</span></span>|<span data-ttu-id="2fa2e-120">管理员为分配筛选器定义的名称。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-120">The admin defined name for assignment filter.</span></span>|
|<span data-ttu-id="2fa2e-121">assignmentFilterPlatform</span><span class="sxs-lookup"><span data-stu-id="2fa2e-121">assignmentFilterPlatform</span></span>|[<span data-ttu-id="2fa2e-122">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="2fa2e-122">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="2fa2e-123">创建此分配筛选器的平台。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-123">The platform for which this assignment filter is created.</span></span> <span data-ttu-id="2fa2e-124">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-124">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="2fa2e-125">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="2fa2e-125">evaluationResult</span></span>|[<span data-ttu-id="2fa2e-126">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="2fa2e-126">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="2fa2e-127">工作分配筛选器评估结果。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-127">Assignment filter evaluation result.</span></span> <span data-ttu-id="2fa2e-128">可取值为：`unknown`、`match`、`notMatch`、`inconclusive`、`failure`、`notEvaluated`。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-128">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|
|<span data-ttu-id="2fa2e-129">evaluationDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa2e-129">evaluationDateTime</span></span>|<span data-ttu-id="2fa2e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa2e-130">DateTimeOffset</span></span>|<span data-ttu-id="2fa2e-131">已评估时间分配筛选器。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-131">The time assignment filter was evaluated.</span></span>|
|<span data-ttu-id="2fa2e-132">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2fa2e-132">assignmentFilterType</span></span>|[<span data-ttu-id="2fa2e-133">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2fa2e-133">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="2fa2e-134">指示包含或排除的筛选器类型。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-134">Indicate filter type either include or exclude.</span></span> <span data-ttu-id="2fa2e-135">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-135">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fa2e-136">关系</span><span class="sxs-lookup"><span data-stu-id="2fa2e-136">Relationships</span></span>
<span data-ttu-id="2fa2e-137">无</span><span class="sxs-lookup"><span data-stu-id="2fa2e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fa2e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fa2e-138">JSON Representation</span></span>
<span data-ttu-id="2fa2e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fa2e-139">Here is a JSON representation of the resource.</span></span>
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
  "assignmentFilterType": "String"
}
```




