---
title: provisioningStep 资源类型
description: '介绍执行操作所执行的步骤。 '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 818063fa078913f694267a9cfb97be649ab81455
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993096"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="c4c77-103">provisioningStep 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4c77-103">provisioningStep resource type</span></span>

<span data-ttu-id="c4c77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4c77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4c77-105">介绍执行操作所执行的步骤。</span><span class="sxs-lookup"><span data-stu-id="c4c77-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="c4c77-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4c77-106">Properties</span></span>

| <span data-ttu-id="c4c77-107">属性</span><span class="sxs-lookup"><span data-stu-id="c4c77-107">Property</span></span>     | <span data-ttu-id="c4c77-108">类型</span><span class="sxs-lookup"><span data-stu-id="c4c77-108">Type</span></span>        | <span data-ttu-id="c4c77-109">说明</span><span class="sxs-lookup"><span data-stu-id="c4c77-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c4c77-110">说明</span><span class="sxs-lookup"><span data-stu-id="c4c77-110">description</span></span>|<span data-ttu-id="c4c77-111">String</span><span class="sxs-lookup"><span data-stu-id="c4c77-111">String</span></span>|<span data-ttu-id="c4c77-112">步骤中发生的操作的摘要。</span><span class="sxs-lookup"><span data-stu-id="c4c77-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="c4c77-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="c4c77-113">details</span></span>|[<span data-ttu-id="c4c77-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="c4c77-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="c4c77-115">步骤中发生的操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c4c77-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="c4c77-116">name</span><span class="sxs-lookup"><span data-stu-id="c4c77-116">name</span></span>|<span data-ttu-id="c4c77-117">String</span><span class="sxs-lookup"><span data-stu-id="c4c77-117">String</span></span>|<span data-ttu-id="c4c77-118">步骤的名称。</span><span class="sxs-lookup"><span data-stu-id="c4c77-118">Name of the step.</span></span>|
|<span data-ttu-id="c4c77-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="c4c77-119">provisioningStepType</span></span>|<span data-ttu-id="c4c77-120">String</span><span class="sxs-lookup"><span data-stu-id="c4c77-120">String</span></span>| <span data-ttu-id="c4c77-121">步骤类型。</span><span class="sxs-lookup"><span data-stu-id="c4c77-121">Type of step.</span></span> <span data-ttu-id="c4c77-122">可取值为：`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c4c77-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c4c77-123">状态</span><span class="sxs-lookup"><span data-stu-id="c4c77-123">status</span></span>|<span data-ttu-id="c4c77-124">String</span><span class="sxs-lookup"><span data-stu-id="c4c77-124">String</span></span>| <span data-ttu-id="c4c77-125">步骤的状态。</span><span class="sxs-lookup"><span data-stu-id="c4c77-125">Status of the step.</span></span> <span data-ttu-id="c4c77-126">可取值为：`success`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c4c77-126">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4c77-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4c77-127">JSON representation</span></span>

<span data-ttu-id="c4c77-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4c77-128">The following is a JSON representation of the resource.</span></span>

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


