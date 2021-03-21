---
title: provisioningStep 资源类型
description: '描述为执行一个操作所执行的步骤。 '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6baf1656cb470cfc8dc01908f5a398ac5d421eb1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960339"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="7eac4-103">provisioningStep 资源类型</span><span class="sxs-lookup"><span data-stu-id="7eac4-103">provisioningStep resource type</span></span>

<span data-ttu-id="7eac4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eac4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7eac4-105">描述为执行一个操作所执行的步骤。</span><span class="sxs-lookup"><span data-stu-id="7eac4-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="7eac4-106">属性</span><span class="sxs-lookup"><span data-stu-id="7eac4-106">Properties</span></span>

| <span data-ttu-id="7eac4-107">属性</span><span class="sxs-lookup"><span data-stu-id="7eac4-107">Property</span></span>     | <span data-ttu-id="7eac4-108">类型</span><span class="sxs-lookup"><span data-stu-id="7eac4-108">Type</span></span>        | <span data-ttu-id="7eac4-109">说明</span><span class="sxs-lookup"><span data-stu-id="7eac4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7eac4-110">说明</span><span class="sxs-lookup"><span data-stu-id="7eac4-110">description</span></span>|<span data-ttu-id="7eac4-111">String</span><span class="sxs-lookup"><span data-stu-id="7eac4-111">String</span></span>|<span data-ttu-id="7eac4-112">步骤中发生的情况摘要。</span><span class="sxs-lookup"><span data-stu-id="7eac4-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="7eac4-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="7eac4-113">details</span></span>|[<span data-ttu-id="7eac4-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="7eac4-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="7eac4-115">步骤中发生的情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7eac4-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="7eac4-116">name</span><span class="sxs-lookup"><span data-stu-id="7eac4-116">name</span></span>|<span data-ttu-id="7eac4-117">String</span><span class="sxs-lookup"><span data-stu-id="7eac4-117">String</span></span>|<span data-ttu-id="7eac4-118">步骤的名称。</span><span class="sxs-lookup"><span data-stu-id="7eac4-118">Name of the step.</span></span>|
|<span data-ttu-id="7eac4-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="7eac4-119">provisioningStepType</span></span>|<span data-ttu-id="7eac4-120">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="7eac4-120">provisioningStepType</span></span>| <span data-ttu-id="7eac4-121">步骤的类型。</span><span class="sxs-lookup"><span data-stu-id="7eac4-121">Type of step.</span></span> <span data-ttu-id="7eac4-122">可取值为：`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7eac4-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7eac4-123">状态</span><span class="sxs-lookup"><span data-stu-id="7eac4-123">status</span></span>|<span data-ttu-id="7eac4-124">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="7eac4-124">provisioningResult</span></span>| <span data-ttu-id="7eac4-125">步骤的状态。</span><span class="sxs-lookup"><span data-stu-id="7eac4-125">Status of the step.</span></span> <span data-ttu-id="7eac4-126">可能的值是 `success` `warning` `failure` ：、、、、。 `skipped` `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="7eac4-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7eac4-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7eac4-127">JSON representation</span></span>

<span data-ttu-id="7eac4-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7eac4-128">The following is a JSON representation of the resource.</span></span>

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


