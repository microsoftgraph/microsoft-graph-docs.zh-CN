---
title: filterOperand 资源类型
description: 包含的操作数值的集合。
ms.openlocfilehash: 8fa4d12efd9fc2b5afa7f250d2ed3f98ed092d06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048167"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="0ac45-103">filterOperand 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ac45-103">filterOperand resource type</span></span>

> <span data-ttu-id="0ac45-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ac45-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ac45-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ac45-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ac45-106">包含的操作数值的集合。</span><span class="sxs-lookup"><span data-stu-id="0ac45-106">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="0ac45-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ac45-107">Properties</span></span>
| <span data-ttu-id="0ac45-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ac45-108">Property</span></span>     | <span data-ttu-id="0ac45-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ac45-109">Type</span></span>   |<span data-ttu-id="0ac45-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ac45-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ac45-111">values</span><span class="sxs-lookup"><span data-stu-id="0ac45-111">values</span></span>|<span data-ttu-id="0ac45-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ac45-112">String collection</span></span>|<span data-ttu-id="0ac45-113">值的集合。</span><span class="sxs-lookup"><span data-stu-id="0ac45-113">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ac45-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ac45-114">JSON representation</span></span>

<span data-ttu-id="0ac45-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ac45-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperand"
}-->

```json
{
  "values": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterOperand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->