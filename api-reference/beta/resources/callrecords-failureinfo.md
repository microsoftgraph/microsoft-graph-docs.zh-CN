---
title: failureInfo 资源类型
description: FailureInfo 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 38ccc3094521283c6c496b1d0e35b97a6cf37199
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353614"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="bc35d-103">failureInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc35d-103">failureInfo resource type</span></span>

<span data-ttu-id="bc35d-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="bc35d-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc35d-105">表示有关呼叫或呼叫的部分失败原因的信息。</span><span class="sxs-lookup"><span data-stu-id="bc35d-105">Represents information about why a call or portion of a call failed.</span></span>

## <a name="properties"></a><span data-ttu-id="bc35d-106">属性</span><span class="sxs-lookup"><span data-stu-id="bc35d-106">Properties</span></span>

| <span data-ttu-id="bc35d-107">属性</span><span class="sxs-lookup"><span data-stu-id="bc35d-107">Property</span></span>     | <span data-ttu-id="bc35d-108">类型</span><span class="sxs-lookup"><span data-stu-id="bc35d-108">Type</span></span>        | <span data-ttu-id="bc35d-109">说明</span><span class="sxs-lookup"><span data-stu-id="bc35d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc35d-110">reason</span><span class="sxs-lookup"><span data-stu-id="bc35d-110">reason</span></span>|<span data-ttu-id="bc35d-111">字符串</span><span class="sxs-lookup"><span data-stu-id="bc35d-111">String</span></span>|<span data-ttu-id="bc35d-112">对呼叫或呼叫部分失败的原因进行分类。</span><span class="sxs-lookup"><span data-stu-id="bc35d-112">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="bc35d-113">交给</span><span class="sxs-lookup"><span data-stu-id="bc35d-113">stage</span></span>|<span data-ttu-id="bc35d-114">callRecords。 failureStage</span><span class="sxs-lookup"><span data-stu-id="bc35d-114">microsoft.graph.callRecords.failureStage</span></span>|<span data-ttu-id="bc35d-115">发生故障时的阶段。</span><span class="sxs-lookup"><span data-stu-id="bc35d-115">The stage when the failure occurred.</span></span> <span data-ttu-id="bc35d-116">可取值为：`unknown`、`callSetup`、`midcall`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="bc35d-116">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc35d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc35d-117">JSON representation</span></span>

<span data-ttu-id="bc35d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc35d-118">The following is a JSON representation of the resource.</span></span>

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