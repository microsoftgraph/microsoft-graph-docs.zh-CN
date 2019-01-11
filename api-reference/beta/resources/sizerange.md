---
title: sizeRange 资源类型
description: 指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。
localization_priority: Normal
ms.openlocfilehash: 14dd86502feb0a5082d3af142202f77ec9eac75c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876403"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="754e0-103">sizeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="754e0-103">sizeRange resource type</span></span>

> <span data-ttu-id="754e0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="754e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="754e0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="754e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="754e0-106">指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="754e0-106">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="754e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="754e0-107">Properties</span></span>
| <span data-ttu-id="754e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="754e0-108">Property</span></span>     | <span data-ttu-id="754e0-109">类型</span><span class="sxs-lookup"><span data-stu-id="754e0-109">Type</span></span>   |<span data-ttu-id="754e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="754e0-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="754e0-111">maximumSize</span><span class="sxs-lookup"><span data-stu-id="754e0-111">maximumSize</span></span> | <span data-ttu-id="754e0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="754e0-112">Int32</span></span> | <span data-ttu-id="754e0-113">传入邮件必须具有的最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="754e0-113">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="754e0-114">minimumSize</span><span class="sxs-lookup"><span data-stu-id="754e0-114">minimumSize</span></span> | <span data-ttu-id="754e0-115">Int32</span><span class="sxs-lookup"><span data-stu-id="754e0-115">Int32</span></span> | <span data-ttu-id="754e0-116">传入邮件必须具有的最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="754e0-116">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="754e0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="754e0-117">JSON representation</span></span>
<span data-ttu-id="754e0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="754e0-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
