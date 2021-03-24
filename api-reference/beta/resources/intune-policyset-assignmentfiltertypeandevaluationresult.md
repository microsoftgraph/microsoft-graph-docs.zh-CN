---
title: assignmentFilterTypeAndEvaluationResult 资源类型
description: 表示筛选器的筛选类型和 evalaution 结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f969660fed52d3bdc3c37643d4502ff722cbee0d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146745"
---
# <a name="assignmentfiltertypeandevaluationresult-resource-type"></a><span data-ttu-id="127c8-103">assignmentFilterTypeAndEvaluationResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="127c8-103">assignmentFilterTypeAndEvaluationResult resource type</span></span>

<span data-ttu-id="127c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="127c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="127c8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="127c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="127c8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="127c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="127c8-107">表示筛选器的筛选类型和 evalaution 结果。</span><span class="sxs-lookup"><span data-stu-id="127c8-107">Represents the filter type and evalaution result of the filter.</span></span>

## <a name="properties"></a><span data-ttu-id="127c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="127c8-108">Properties</span></span>
|<span data-ttu-id="127c8-109">属性</span><span class="sxs-lookup"><span data-stu-id="127c8-109">Property</span></span>|<span data-ttu-id="127c8-110">类型</span><span class="sxs-lookup"><span data-stu-id="127c8-110">Type</span></span>|<span data-ttu-id="127c8-111">说明</span><span class="sxs-lookup"><span data-stu-id="127c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="127c8-112">assignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="127c8-112">assignmentFilterType</span></span>|[<span data-ttu-id="127c8-113">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="127c8-113">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="127c8-114">表示筛选器类型。</span><span class="sxs-lookup"><span data-stu-id="127c8-114">Represents the filter type.</span></span> <span data-ttu-id="127c8-115">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="127c8-115">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="127c8-116">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="127c8-116">evaluationResult</span></span>|[<span data-ttu-id="127c8-117">assignmentFilterEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="127c8-117">assignmentFilterEvaluationResult</span></span>](../resources/intune-policyset-assignmentfilterevaluationresult.md)|<span data-ttu-id="127c8-118">表示筛选器的 evalaution 结果。</span><span class="sxs-lookup"><span data-stu-id="127c8-118">Represents the evalaution result of the filter.</span></span> <span data-ttu-id="127c8-119">可取值为：`unknown`、`match`、`notMatch`、`inconclusive`、`failure`、`notEvaluated`。</span><span class="sxs-lookup"><span data-stu-id="127c8-119">Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="127c8-120">关系</span><span class="sxs-lookup"><span data-stu-id="127c8-120">Relationships</span></span>
<span data-ttu-id="127c8-121">无</span><span class="sxs-lookup"><span data-stu-id="127c8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="127c8-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="127c8-122">JSON Representation</span></span>
<span data-ttu-id="127c8-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="127c8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterTypeAndEvaluationResult",
  "assignmentFilterType": "String",
  "evaluationResult": "String"
}
```




