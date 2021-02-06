---
title: sizeRange 资源类型
description: 指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: af63282d3093fc0178dba6027846b2c080c3c5f9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136925"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="02a60-103">sizeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="02a60-103">sizeRange resource type</span></span>

<span data-ttu-id="02a60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02a60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a60-105">指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="02a60-105">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="02a60-106">属性</span><span class="sxs-lookup"><span data-stu-id="02a60-106">Properties</span></span>
| <span data-ttu-id="02a60-107">属性</span><span class="sxs-lookup"><span data-stu-id="02a60-107">Property</span></span>     | <span data-ttu-id="02a60-108">类型</span><span class="sxs-lookup"><span data-stu-id="02a60-108">Type</span></span>   |<span data-ttu-id="02a60-109">说明</span><span class="sxs-lookup"><span data-stu-id="02a60-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="02a60-110">maximumSize</span><span class="sxs-lookup"><span data-stu-id="02a60-110">maximumSize</span></span> | <span data-ttu-id="02a60-111">Int32</span><span class="sxs-lookup"><span data-stu-id="02a60-111">Int32</span></span> | <span data-ttu-id="02a60-112">传入邮件必须具有的最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="02a60-112">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="02a60-113">minimumSize</span><span class="sxs-lookup"><span data-stu-id="02a60-113">minimumSize</span></span> | <span data-ttu-id="02a60-114">Int32</span><span class="sxs-lookup"><span data-stu-id="02a60-114">Int32</span></span> | <span data-ttu-id="02a60-115">传入邮件必须具有的最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="02a60-115">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="02a60-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02a60-116">JSON representation</span></span>
<span data-ttu-id="02a60-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02a60-117">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


