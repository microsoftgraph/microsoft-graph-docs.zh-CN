---
title: convertIdResult 资源类型
description: translateExchangeIds 函数执行的 ID 格式转换的结果。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 1710c437421426b4bd072e3c654df7d076d0f9f7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135152"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="28d69-103">convertIdResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="28d69-103">convertIdResult resource type</span></span>

<span data-ttu-id="28d69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28d69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28d69-105">[translateExchangeIds](../api/user-translateexchangeids.md)函数执行的 ID 格式转换的结果。</span><span class="sxs-lookup"><span data-stu-id="28d69-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="28d69-106">属性</span><span class="sxs-lookup"><span data-stu-id="28d69-106">Properties</span></span>

| <span data-ttu-id="28d69-107">属性</span><span class="sxs-lookup"><span data-stu-id="28d69-107">Property</span></span> | <span data-ttu-id="28d69-108">类型</span><span class="sxs-lookup"><span data-stu-id="28d69-108">Type</span></span> | <span data-ttu-id="28d69-109">说明</span><span class="sxs-lookup"><span data-stu-id="28d69-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="28d69-110">sourceId</span><span class="sxs-lookup"><span data-stu-id="28d69-110">sourceId</span></span> | <span data-ttu-id="28d69-111">String</span><span class="sxs-lookup"><span data-stu-id="28d69-111">String</span></span> | <span data-ttu-id="28d69-112">已转换的标识符。</span><span class="sxs-lookup"><span data-stu-id="28d69-112">The identifier that was converted.</span></span> <span data-ttu-id="28d69-113">此值为原始的未转换标识符。</span><span class="sxs-lookup"><span data-stu-id="28d69-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="28d69-114">targetId</span><span class="sxs-lookup"><span data-stu-id="28d69-114">targetId</span></span> | <span data-ttu-id="28d69-115">String</span><span class="sxs-lookup"><span data-stu-id="28d69-115">String</span></span> | <span data-ttu-id="28d69-116">转换后的标识符。</span><span class="sxs-lookup"><span data-stu-id="28d69-116">The converted identifier.</span></span> <span data-ttu-id="28d69-117">如果转换失败，则此值不存在。</span><span class="sxs-lookup"><span data-stu-id="28d69-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="28d69-118">errorDetails</span><span class="sxs-lookup"><span data-stu-id="28d69-118">errorDetails</span></span> | [<span data-ttu-id="28d69-119">genericError</span><span class="sxs-lookup"><span data-stu-id="28d69-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="28d69-120">指示转换失败原因的错误对象。</span><span class="sxs-lookup"><span data-stu-id="28d69-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="28d69-121">如果转换成功，则此值不存在。</span><span class="sxs-lookup"><span data-stu-id="28d69-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="28d69-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28d69-122">JSON representation</span></span>

<span data-ttu-id="28d69-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28d69-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```

