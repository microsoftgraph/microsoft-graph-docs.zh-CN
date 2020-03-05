---
title: convertIdResult 资源类型
description: 由 translateExchangeIds 函数执行的 ID 格式转换的结果。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 6c4cd63316747b51474dd5c61912c0f155c047c8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507385"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="621cf-103">convertIdResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="621cf-103">convertIdResult resource type</span></span>

<span data-ttu-id="621cf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="621cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="621cf-105">由[translateExchangeIds](../api/user-translateexchangeids.md)函数执行的 ID 格式转换的结果。</span><span class="sxs-lookup"><span data-stu-id="621cf-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="621cf-106">属性</span><span class="sxs-lookup"><span data-stu-id="621cf-106">Properties</span></span>

| <span data-ttu-id="621cf-107">属性</span><span class="sxs-lookup"><span data-stu-id="621cf-107">Property</span></span> | <span data-ttu-id="621cf-108">类型</span><span class="sxs-lookup"><span data-stu-id="621cf-108">Type</span></span> | <span data-ttu-id="621cf-109">说明</span><span class="sxs-lookup"><span data-stu-id="621cf-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="621cf-110">sourceId</span><span class="sxs-lookup"><span data-stu-id="621cf-110">sourceId</span></span> | <span data-ttu-id="621cf-111">String</span><span class="sxs-lookup"><span data-stu-id="621cf-111">String</span></span> | <span data-ttu-id="621cf-112">已转换的标识符。</span><span class="sxs-lookup"><span data-stu-id="621cf-112">The identifier that was converted.</span></span> <span data-ttu-id="621cf-113">此值是未转换的原始标识符。</span><span class="sxs-lookup"><span data-stu-id="621cf-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="621cf-114">targetId</span><span class="sxs-lookup"><span data-stu-id="621cf-114">targetId</span></span> | <span data-ttu-id="621cf-115">String</span><span class="sxs-lookup"><span data-stu-id="621cf-115">String</span></span> | <span data-ttu-id="621cf-116">转换后的标识符。</span><span class="sxs-lookup"><span data-stu-id="621cf-116">The converted identifier.</span></span> <span data-ttu-id="621cf-117">如果转换失败，则不会出现此值。</span><span class="sxs-lookup"><span data-stu-id="621cf-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="621cf-118">errorDetails</span><span class="sxs-lookup"><span data-stu-id="621cf-118">errorDetails</span></span> | [<span data-ttu-id="621cf-119">genericError</span><span class="sxs-lookup"><span data-stu-id="621cf-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="621cf-120">一个指示转换失败原因的 error 对象。</span><span class="sxs-lookup"><span data-stu-id="621cf-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="621cf-121">如果转换成功，则不会出现此值。</span><span class="sxs-lookup"><span data-stu-id="621cf-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="621cf-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="621cf-122">JSON representation</span></span>

<span data-ttu-id="621cf-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="621cf-123">Here is a JSON representation of the resource.</span></span>

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
