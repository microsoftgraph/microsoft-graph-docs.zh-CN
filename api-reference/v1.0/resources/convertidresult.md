---
title: convertIdResult 资源类型
description: 由 translateExchangeIds 函数执行的 ID 格式转换的结果。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 405d663e4f1f7fb040e79cdd10669bc824e3edef
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036443"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="9b170-103">convertIdResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b170-103">convertIdResult resource type</span></span>

<span data-ttu-id="9b170-104">由[translateExchangeIds](../api/user-translateexchangeids.md)函数执行的 ID 格式转换的结果。</span><span class="sxs-lookup"><span data-stu-id="9b170-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="9b170-105">属性</span><span class="sxs-lookup"><span data-stu-id="9b170-105">Properties</span></span>

| <span data-ttu-id="9b170-106">属性</span><span class="sxs-lookup"><span data-stu-id="9b170-106">Property</span></span> | <span data-ttu-id="9b170-107">类型</span><span class="sxs-lookup"><span data-stu-id="9b170-107">Type</span></span> | <span data-ttu-id="9b170-108">说明</span><span class="sxs-lookup"><span data-stu-id="9b170-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="9b170-109">sourceId</span><span class="sxs-lookup"><span data-stu-id="9b170-109">sourceId</span></span> | <span data-ttu-id="9b170-110">String</span><span class="sxs-lookup"><span data-stu-id="9b170-110">String</span></span> | <span data-ttu-id="9b170-111">已转换的标识符。</span><span class="sxs-lookup"><span data-stu-id="9b170-111">The identifier that was converted.</span></span> <span data-ttu-id="9b170-112">此值是未转换的原始标识符。</span><span class="sxs-lookup"><span data-stu-id="9b170-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="9b170-113">targetId</span><span class="sxs-lookup"><span data-stu-id="9b170-113">targetId</span></span> | <span data-ttu-id="9b170-114">String</span><span class="sxs-lookup"><span data-stu-id="9b170-114">String</span></span> | <span data-ttu-id="9b170-115">转换后的标识符。</span><span class="sxs-lookup"><span data-stu-id="9b170-115">The converted identifier.</span></span> <span data-ttu-id="9b170-116">如果转换失败，则不会出现此值。</span><span class="sxs-lookup"><span data-stu-id="9b170-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="9b170-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="9b170-117">errorDetails</span></span> | [<span data-ttu-id="9b170-118">genericError</span><span class="sxs-lookup"><span data-stu-id="9b170-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="9b170-119">一个指示转换失败原因的 error 对象。</span><span class="sxs-lookup"><span data-stu-id="9b170-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="9b170-120">如果转换成功，则不会出现此值。</span><span class="sxs-lookup"><span data-stu-id="9b170-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9b170-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b170-121">JSON representation</span></span>

<span data-ttu-id="9b170-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b170-122">Here is a JSON representation of the resource.</span></span>

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
