---
title: failureInfo 资源类型
description: FailureInfo 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f32d0b29c62ac5f3fd9b022c550d9715756adca3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601347"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="5738e-103">failureInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5738e-103">failureInfo resource type</span></span>

<span data-ttu-id="5738e-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="5738e-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="5738e-105">表示有关呼叫或呼叫的部分失败原因的信息。</span><span class="sxs-lookup"><span data-stu-id="5738e-105">Represents information about why a call or portion of a call failed.</span></span>

## <a name="properties"></a><span data-ttu-id="5738e-106">属性</span><span class="sxs-lookup"><span data-stu-id="5738e-106">Properties</span></span>

| <span data-ttu-id="5738e-107">属性</span><span class="sxs-lookup"><span data-stu-id="5738e-107">Property</span></span>     | <span data-ttu-id="5738e-108">类型</span><span class="sxs-lookup"><span data-stu-id="5738e-108">Type</span></span>        | <span data-ttu-id="5738e-109">说明</span><span class="sxs-lookup"><span data-stu-id="5738e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5738e-110">reason</span><span class="sxs-lookup"><span data-stu-id="5738e-110">reason</span></span>|<span data-ttu-id="5738e-111">String</span><span class="sxs-lookup"><span data-stu-id="5738e-111">String</span></span>|<span data-ttu-id="5738e-112">对呼叫或呼叫部分失败的原因进行分类。</span><span class="sxs-lookup"><span data-stu-id="5738e-112">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="5738e-113">交给</span><span class="sxs-lookup"><span data-stu-id="5738e-113">stage</span></span>|<span data-ttu-id="5738e-114">callRecords。 failureStage</span><span class="sxs-lookup"><span data-stu-id="5738e-114">microsoft.graph.callRecords.failureStage</span></span>|<span data-ttu-id="5738e-115">发生故障时的阶段。</span><span class="sxs-lookup"><span data-stu-id="5738e-115">The stage when the failure occurred.</span></span> <span data-ttu-id="5738e-116">可取值为：`unknown`、`callSetup`、`midcall`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="5738e-116">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5738e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5738e-117">JSON representation</span></span>

<span data-ttu-id="5738e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5738e-118">The following is a JSON representation of the resource.</span></span>

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
