---
title: provisioningStep 资源类型
description: '描述为执行一个操作所执行的步骤。 '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 695f0c30e802dabb03cb30f0615ee6a59e8cc540
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241492"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="03452-103">provisioningStep 资源类型</span><span class="sxs-lookup"><span data-stu-id="03452-103">provisioningStep resource type</span></span>

<span data-ttu-id="03452-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03452-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03452-105">描述为执行一个操作所执行的步骤。</span><span class="sxs-lookup"><span data-stu-id="03452-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="03452-106">属性</span><span class="sxs-lookup"><span data-stu-id="03452-106">Properties</span></span>

| <span data-ttu-id="03452-107">属性</span><span class="sxs-lookup"><span data-stu-id="03452-107">Property</span></span>     | <span data-ttu-id="03452-108">类型</span><span class="sxs-lookup"><span data-stu-id="03452-108">Type</span></span>        | <span data-ttu-id="03452-109">说明</span><span class="sxs-lookup"><span data-stu-id="03452-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03452-110">说明</span><span class="sxs-lookup"><span data-stu-id="03452-110">description</span></span>|<span data-ttu-id="03452-111">String</span><span class="sxs-lookup"><span data-stu-id="03452-111">String</span></span>|<span data-ttu-id="03452-112">步骤中发生的情况摘要。</span><span class="sxs-lookup"><span data-stu-id="03452-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="03452-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="03452-113">details</span></span>|[<span data-ttu-id="03452-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="03452-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="03452-115">步骤中发生的情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="03452-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="03452-116">name</span><span class="sxs-lookup"><span data-stu-id="03452-116">name</span></span>|<span data-ttu-id="03452-117">String</span><span class="sxs-lookup"><span data-stu-id="03452-117">String</span></span>|<span data-ttu-id="03452-118">步骤的名称。</span><span class="sxs-lookup"><span data-stu-id="03452-118">Name of the step.</span></span>|
|<span data-ttu-id="03452-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="03452-119">provisioningStepType</span></span>|<span data-ttu-id="03452-120">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="03452-120">provisioningStepType</span></span>| <span data-ttu-id="03452-121">步骤的类型。</span><span class="sxs-lookup"><span data-stu-id="03452-121">Type of step.</span></span> <span data-ttu-id="03452-122">可取值为：`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="03452-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="03452-123">状态</span><span class="sxs-lookup"><span data-stu-id="03452-123">status</span></span>|<span data-ttu-id="03452-124">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="03452-124">provisioningResult</span></span>| <span data-ttu-id="03452-125">步骤的状态。</span><span class="sxs-lookup"><span data-stu-id="03452-125">Status of the step.</span></span> <span data-ttu-id="03452-126">可能的值是 `success` `warning` `failure` ：、、、、。 `skipped` `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="03452-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03452-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03452-127">JSON representation</span></span>

<span data-ttu-id="03452-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03452-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


