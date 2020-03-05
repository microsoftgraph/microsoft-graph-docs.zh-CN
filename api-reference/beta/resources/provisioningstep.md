---
title: provisioningStep 资源类型
description: '介绍执行操作所执行的步骤。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4275730cfd7c9c9c58496b674062ffedb5d7a6cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521325"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="4a200-103">provisioningStep 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a200-103">provisioningStep resource type</span></span>

<span data-ttu-id="4a200-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4a200-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a200-105">介绍执行操作所执行的步骤。</span><span class="sxs-lookup"><span data-stu-id="4a200-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="4a200-106">属性</span><span class="sxs-lookup"><span data-stu-id="4a200-106">Properties</span></span>

| <span data-ttu-id="4a200-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a200-107">Property</span></span>     | <span data-ttu-id="4a200-108">类型</span><span class="sxs-lookup"><span data-stu-id="4a200-108">Type</span></span>        | <span data-ttu-id="4a200-109">说明</span><span class="sxs-lookup"><span data-stu-id="4a200-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a200-110">说明</span><span class="sxs-lookup"><span data-stu-id="4a200-110">description</span></span>|<span data-ttu-id="4a200-111">String</span><span class="sxs-lookup"><span data-stu-id="4a200-111">String</span></span>|<span data-ttu-id="4a200-112">步骤中发生的操作的摘要。</span><span class="sxs-lookup"><span data-stu-id="4a200-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="4a200-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="4a200-113">details</span></span>|[<span data-ttu-id="4a200-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="4a200-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="4a200-115">步骤中发生的操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4a200-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="4a200-116">name</span><span class="sxs-lookup"><span data-stu-id="4a200-116">name</span></span>|<span data-ttu-id="4a200-117">字符串</span><span class="sxs-lookup"><span data-stu-id="4a200-117">String</span></span>|<span data-ttu-id="4a200-118">步骤的名称。</span><span class="sxs-lookup"><span data-stu-id="4a200-118">Name of the step.</span></span>|
|<span data-ttu-id="4a200-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="4a200-119">provisioningStepType</span></span>|<span data-ttu-id="4a200-120">String</span><span class="sxs-lookup"><span data-stu-id="4a200-120">String</span></span>| <span data-ttu-id="4a200-121">步骤类型。</span><span class="sxs-lookup"><span data-stu-id="4a200-121">Type of step.</span></span> <span data-ttu-id="4a200-122">可取值为：`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4a200-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4a200-123">status</span><span class="sxs-lookup"><span data-stu-id="4a200-123">status</span></span>|<span data-ttu-id="4a200-124">String</span><span class="sxs-lookup"><span data-stu-id="4a200-124">String</span></span>| <span data-ttu-id="4a200-125">步骤的状态。</span><span class="sxs-lookup"><span data-stu-id="4a200-125">Status of the step.</span></span> <span data-ttu-id="4a200-126">可取值为：`success`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4a200-126">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a200-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a200-127">JSON representation</span></span>

<span data-ttu-id="4a200-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a200-128">The following is a JSON representation of the resource.</span></span>

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
