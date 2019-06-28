---
title: provisioningStep 资源类型
description: '介绍执行操作所执行的步骤。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1658114615c4532f0a7f9b9f5ad3c3a25deff81b
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349341"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="edcbf-103">provisioningStep 资源类型</span><span class="sxs-lookup"><span data-stu-id="edcbf-103">provisioningStep resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edcbf-104">介绍执行操作所执行的步骤。</span><span class="sxs-lookup"><span data-stu-id="edcbf-104">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="edcbf-105">属性</span><span class="sxs-lookup"><span data-stu-id="edcbf-105">Properties</span></span>

| <span data-ttu-id="edcbf-106">属性</span><span class="sxs-lookup"><span data-stu-id="edcbf-106">Property</span></span>     | <span data-ttu-id="edcbf-107">类型</span><span class="sxs-lookup"><span data-stu-id="edcbf-107">Type</span></span>        | <span data-ttu-id="edcbf-108">说明</span><span class="sxs-lookup"><span data-stu-id="edcbf-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="edcbf-109">说明</span><span class="sxs-lookup"><span data-stu-id="edcbf-109">description</span></span>|<span data-ttu-id="edcbf-110">String</span><span class="sxs-lookup"><span data-stu-id="edcbf-110">String</span></span>|<span data-ttu-id="edcbf-111">步骤中发生的操作的摘要。</span><span class="sxs-lookup"><span data-stu-id="edcbf-111">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="edcbf-112">详细信息</span><span class="sxs-lookup"><span data-stu-id="edcbf-112">details</span></span>|[<span data-ttu-id="edcbf-113">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="edcbf-113">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="edcbf-114">步骤中发生的操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="edcbf-114">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="edcbf-115">name</span><span class="sxs-lookup"><span data-stu-id="edcbf-115">name</span></span>|<span data-ttu-id="edcbf-116">字符串</span><span class="sxs-lookup"><span data-stu-id="edcbf-116">String</span></span>|<span data-ttu-id="edcbf-117">步骤的名称。</span><span class="sxs-lookup"><span data-stu-id="edcbf-117">Name of the step.</span></span>|
|<span data-ttu-id="edcbf-118">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="edcbf-118">provisioningStepType</span></span>|<span data-ttu-id="edcbf-119">String</span><span class="sxs-lookup"><span data-stu-id="edcbf-119">String</span></span>| <span data-ttu-id="edcbf-120">步骤类型。</span><span class="sxs-lookup"><span data-stu-id="edcbf-120">Type of step.</span></span> <span data-ttu-id="edcbf-121">可取值为：`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="edcbf-121">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="edcbf-122">status</span><span class="sxs-lookup"><span data-stu-id="edcbf-122">status</span></span>|<span data-ttu-id="edcbf-123">String</span><span class="sxs-lookup"><span data-stu-id="edcbf-123">String</span></span>| <span data-ttu-id="edcbf-124">步骤的状态。</span><span class="sxs-lookup"><span data-stu-id="edcbf-124">Status of the step.</span></span> <span data-ttu-id="edcbf-125">可取值为：`success`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="edcbf-125">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edcbf-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edcbf-126">JSON representation</span></span>

<span data-ttu-id="edcbf-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edcbf-127">The following is a JSON representation of the resource.</span></span>

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
