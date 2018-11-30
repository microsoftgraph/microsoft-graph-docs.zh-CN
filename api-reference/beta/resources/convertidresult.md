---
title: convertIdResult 资源类型
description: 执行由 translateExchangeIds 函数 ID 格式转换的结果。
ms.openlocfilehash: 3a17399ffe44c43c78f7b50933b2e847a3e64f32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042804"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="4dec3-103">convertIdResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="4dec3-103">convertIdResult resource type</span></span>

> <span data-ttu-id="4dec3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4dec3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dec3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4dec3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4dec3-106">执行由[translateExchangeIds](../api/user-translateexchangeids.md)函数 ID 格式转换的结果。</span><span class="sxs-lookup"><span data-stu-id="4dec3-106">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="4dec3-107">属性</span><span class="sxs-lookup"><span data-stu-id="4dec3-107">Properties</span></span>

| <span data-ttu-id="4dec3-108">属性</span><span class="sxs-lookup"><span data-stu-id="4dec3-108">Property</span></span> | <span data-ttu-id="4dec3-109">类型</span><span class="sxs-lookup"><span data-stu-id="4dec3-109">Type</span></span> | <span data-ttu-id="4dec3-110">说明</span><span class="sxs-lookup"><span data-stu-id="4dec3-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="4dec3-111">sourceId</span><span class="sxs-lookup"><span data-stu-id="4dec3-111">sourceId</span></span> | <span data-ttu-id="4dec3-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4dec3-112">String</span></span> | <span data-ttu-id="4dec3-113">已转换的标识符。</span><span class="sxs-lookup"><span data-stu-id="4dec3-113">The identifier that was converted.</span></span> <span data-ttu-id="4dec3-114">此值是原始、 未转换标识符。</span><span class="sxs-lookup"><span data-stu-id="4dec3-114">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="4dec3-115">targetId</span><span class="sxs-lookup"><span data-stu-id="4dec3-115">targetId</span></span> | <span data-ttu-id="4dec3-116">字符串</span><span class="sxs-lookup"><span data-stu-id="4dec3-116">String</span></span> | <span data-ttu-id="4dec3-117">转换后的标识符。</span><span class="sxs-lookup"><span data-stu-id="4dec3-117">The converted identifier.</span></span> <span data-ttu-id="4dec3-118">此值不存在，如果转换失败。</span><span class="sxs-lookup"><span data-stu-id="4dec3-118">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="4dec3-119">errorDetails</span><span class="sxs-lookup"><span data-stu-id="4dec3-119">errorDetails</span></span> | [<span data-ttu-id="4dec3-120">genericError</span><span class="sxs-lookup"><span data-stu-id="4dec3-120">genericError</span></span>](genericerror.md) | <span data-ttu-id="4dec3-121">Error 对象指示转换失败的原因。</span><span class="sxs-lookup"><span data-stu-id="4dec3-121">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="4dec3-122">此值不存在，如果转换成功。</span><span class="sxs-lookup"><span data-stu-id="4dec3-122">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4dec3-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4dec3-123">JSON representation</span></span>

<span data-ttu-id="4dec3-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dec3-124">Here is a JSON representation of the resource.</span></span>

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