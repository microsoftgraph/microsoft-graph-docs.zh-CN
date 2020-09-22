---
title: failureInfo 资源类型
description: FailureInfo 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5edd2a501b3e1a5633f0bd01ac36815201eb927d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064372"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="50801-103">failureInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="50801-103">failureInfo resource type</span></span>

<span data-ttu-id="50801-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="50801-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50801-105">表示有关呼叫或呼叫的部分失败原因的信息。</span><span class="sxs-lookup"><span data-stu-id="50801-105">Represents information about why a call or portion of a call failed.</span></span>

<span data-ttu-id="50801-106">故障可分为两种类型：</span><span class="sxs-lookup"><span data-stu-id="50801-106">The failure can be of two types:</span></span> 

- <span data-ttu-id="50801-107">呼叫设置失败</span><span class="sxs-lookup"><span data-stu-id="50801-107">Call setup failure</span></span>
- <span data-ttu-id="50801-108">中/呼叫删除</span><span class="sxs-lookup"><span data-stu-id="50801-108">Mid-call drop</span></span>

<span data-ttu-id="50801-109">如果一个或多个媒体流具有这些故障中的任何一个，则会在分段级别传播该故障。</span><span class="sxs-lookup"><span data-stu-id="50801-109">If one or more media streams have any of these failures, that failure is propagated at the segment level.</span></span> <span data-ttu-id="50801-110">如果一个或多个段具有这些故障中的任何一个，则会在会话级别传播该故障。</span><span class="sxs-lookup"><span data-stu-id="50801-110">If one or more segments have any of these failures, that failure is propagated at the session level.</span></span>

## <a name="properties"></a><span data-ttu-id="50801-111">属性</span><span class="sxs-lookup"><span data-stu-id="50801-111">Properties</span></span>

| <span data-ttu-id="50801-112">属性</span><span class="sxs-lookup"><span data-stu-id="50801-112">Property</span></span>     | <span data-ttu-id="50801-113">类型</span><span class="sxs-lookup"><span data-stu-id="50801-113">Type</span></span>        | <span data-ttu-id="50801-114">说明</span><span class="sxs-lookup"><span data-stu-id="50801-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50801-115">reason</span><span class="sxs-lookup"><span data-stu-id="50801-115">reason</span></span>|<span data-ttu-id="50801-116">String</span><span class="sxs-lookup"><span data-stu-id="50801-116">String</span></span>|<span data-ttu-id="50801-117">对呼叫或呼叫部分失败的原因进行分类。</span><span class="sxs-lookup"><span data-stu-id="50801-117">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="50801-118">交给</span><span class="sxs-lookup"><span data-stu-id="50801-118">stage</span></span>|<span data-ttu-id="50801-119">callRecords。 failureStage</span><span class="sxs-lookup"><span data-stu-id="50801-119">microsoft.graph.callRecords.failureStage</span></span>|<span data-ttu-id="50801-120">发生故障时的阶段。</span><span class="sxs-lookup"><span data-stu-id="50801-120">The stage when the failure occurred.</span></span> <span data-ttu-id="50801-121">可取值为：`unknown`、`callSetup`、`midcall`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="50801-121">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50801-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50801-122">JSON representation</span></span>

<span data-ttu-id="50801-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50801-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.failureInfo",
  "baseType": null
}-->

```json
{
  "reason": "String",
  "stage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "failureInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


