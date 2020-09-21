---
title: sizeRange 资源类型
description: 指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 223a58abf7d95761e316e39468be12f858db49dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063938"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="bfa88-103">sizeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfa88-103">sizeRange resource type</span></span>

<span data-ttu-id="bfa88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfa88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfa88-105">指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="bfa88-105">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="bfa88-106">属性</span><span class="sxs-lookup"><span data-stu-id="bfa88-106">Properties</span></span>
| <span data-ttu-id="bfa88-107">属性</span><span class="sxs-lookup"><span data-stu-id="bfa88-107">Property</span></span>     | <span data-ttu-id="bfa88-108">类型</span><span class="sxs-lookup"><span data-stu-id="bfa88-108">Type</span></span>   |<span data-ttu-id="bfa88-109">说明</span><span class="sxs-lookup"><span data-stu-id="bfa88-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bfa88-110">maximumSize</span><span class="sxs-lookup"><span data-stu-id="bfa88-110">maximumSize</span></span> | <span data-ttu-id="bfa88-111">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa88-111">Int32</span></span> | <span data-ttu-id="bfa88-112">传入邮件必须具有的最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="bfa88-112">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="bfa88-113">minimumSize</span><span class="sxs-lookup"><span data-stu-id="bfa88-113">minimumSize</span></span> | <span data-ttu-id="bfa88-114">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa88-114">Int32</span></span> | <span data-ttu-id="bfa88-115">传入邮件必须具有的最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="bfa88-115">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="bfa88-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfa88-116">JSON representation</span></span>
<span data-ttu-id="bfa88-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfa88-117">Here is a JSON representation of the resource.</span></span>

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


