---
title: sizeRange 资源类型
description: 指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7eed9cfdd4739ee35c340d0cfeaeb8cc6d088455
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137079"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="82672-103">sizeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="82672-103">sizeRange resource type</span></span>

<span data-ttu-id="82672-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82672-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="82672-105">指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="82672-105">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="82672-106">属性</span><span class="sxs-lookup"><span data-stu-id="82672-106">Properties</span></span>
| <span data-ttu-id="82672-107">属性</span><span class="sxs-lookup"><span data-stu-id="82672-107">Property</span></span>     | <span data-ttu-id="82672-108">类型</span><span class="sxs-lookup"><span data-stu-id="82672-108">Type</span></span>   |<span data-ttu-id="82672-109">说明</span><span class="sxs-lookup"><span data-stu-id="82672-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="82672-110">maximumSize</span><span class="sxs-lookup"><span data-stu-id="82672-110">maximumSize</span></span> | <span data-ttu-id="82672-111">Int32</span><span class="sxs-lookup"><span data-stu-id="82672-111">Int32</span></span> | <span data-ttu-id="82672-112">传入邮件必须具有的最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="82672-112">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="82672-113">minimumSize</span><span class="sxs-lookup"><span data-stu-id="82672-113">minimumSize</span></span> | <span data-ttu-id="82672-114">Int32</span><span class="sxs-lookup"><span data-stu-id="82672-114">Int32</span></span> | <span data-ttu-id="82672-115">传入邮件必须具有的最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="82672-115">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="82672-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82672-116">JSON representation</span></span>
<span data-ttu-id="82672-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82672-117">Here is a JSON representation of the resource.</span></span>

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

