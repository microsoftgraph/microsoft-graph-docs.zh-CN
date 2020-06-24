---
title: printDocument 资源类型
description: 代表要打印的文档。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 1e7a1d6a9c131417e4f0ef171ac364e5fe8b106b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863780"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="d5db9-103">printDocument 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5db9-103">printDocument resource type</span></span>

<span data-ttu-id="d5db9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5db9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5db9-105">代表要打印的文档。</span><span class="sxs-lookup"><span data-stu-id="d5db9-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="d5db9-106">Methods</span><span class="sxs-lookup"><span data-stu-id="d5db9-106">Methods</span></span>

| <span data-ttu-id="d5db9-107">方法</span><span class="sxs-lookup"><span data-stu-id="d5db9-107">Method</span></span>       | <span data-ttu-id="d5db9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5db9-108">Return Type</span></span> | <span data-ttu-id="d5db9-109">说明</span><span class="sxs-lookup"><span data-stu-id="d5db9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d5db9-110">uploadData</span><span class="sxs-lookup"><span data-stu-id="d5db9-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="d5db9-111">无</span><span class="sxs-lookup"><span data-stu-id="d5db9-111">None</span></span> | <span data-ttu-id="d5db9-112">上载**printDocument**的单个二进制段。</span><span class="sxs-lookup"><span data-stu-id="d5db9-112">Upload a single binary segment of the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="d5db9-113">属性</span><span class="sxs-lookup"><span data-stu-id="d5db9-113">Properties</span></span>
| <span data-ttu-id="d5db9-114">属性</span><span class="sxs-lookup"><span data-stu-id="d5db9-114">Property</span></span>     | <span data-ttu-id="d5db9-115">类型</span><span class="sxs-lookup"><span data-stu-id="d5db9-115">Type</span></span>        | <span data-ttu-id="d5db9-116">说明</span><span class="sxs-lookup"><span data-stu-id="d5db9-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d5db9-117">id</span><span class="sxs-lookup"><span data-stu-id="d5db9-117">id</span></span>|<span data-ttu-id="d5db9-118">字符串</span><span class="sxs-lookup"><span data-stu-id="d5db9-118">String</span></span>|<span data-ttu-id="d5db9-119">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="d5db9-119">The document's identifier.</span></span> <span data-ttu-id="d5db9-120">只读。</span><span class="sxs-lookup"><span data-stu-id="d5db9-120">Read-only.</span></span>|
|<span data-ttu-id="d5db9-121">displayName</span><span class="sxs-lookup"><span data-stu-id="d5db9-121">displayName</span></span>|<span data-ttu-id="d5db9-122">String</span><span class="sxs-lookup"><span data-stu-id="d5db9-122">String</span></span>|<span data-ttu-id="d5db9-123">文档的名称。</span><span class="sxs-lookup"><span data-stu-id="d5db9-123">The document's name.</span></span> <span data-ttu-id="d5db9-124">只读。</span><span class="sxs-lookup"><span data-stu-id="d5db9-124">Read-only.</span></span>|
|<span data-ttu-id="d5db9-125">contentType</span><span class="sxs-lookup"><span data-stu-id="d5db9-125">contentType</span></span>|<span data-ttu-id="d5db9-126">String</span><span class="sxs-lookup"><span data-stu-id="d5db9-126">String</span></span>|<span data-ttu-id="d5db9-127">文档的内容（MIME）类型。</span><span class="sxs-lookup"><span data-stu-id="d5db9-127">The document's content (MIME) type.</span></span> <span data-ttu-id="d5db9-128">只读。</span><span class="sxs-lookup"><span data-stu-id="d5db9-128">Read-only.</span></span>|
|<span data-ttu-id="d5db9-129">size</span><span class="sxs-lookup"><span data-stu-id="d5db9-129">size</span></span>|<span data-ttu-id="d5db9-130">Int64</span><span class="sxs-lookup"><span data-stu-id="d5db9-130">Int64</span></span>|<span data-ttu-id="d5db9-131">文档的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="d5db9-131">The document's size in bytes.</span></span> <span data-ttu-id="d5db9-132">只读。</span><span class="sxs-lookup"><span data-stu-id="d5db9-132">Read-only.</span></span>|
|<span data-ttu-id="d5db9-133">configuration</span><span class="sxs-lookup"><span data-stu-id="d5db9-133">configuration</span></span>|[<span data-ttu-id="d5db9-134">printerDocumentConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5db9-134">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="d5db9-135">打印机打印文档时应使用的一组设置。</span><span class="sxs-lookup"><span data-stu-id="d5db9-135">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="d5db9-136">只读。</span><span class="sxs-lookup"><span data-stu-id="d5db9-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5db9-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5db9-137">JSON representation</span></span>

<span data-ttu-id="d5db9-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5db9-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "mimeType": "String",
  "sizeInBytes": 12345,
  "documentConfiguration": {
    "pageRanges": [ {"@odata.type": "microsoft.graph.printPageRange"} ],
    "printQuality": "String",
    "printResolutionInDpi": 123456,
    "feedDirection": "String",
    "orientation": "String",
    "duplexConfiguration": "String",
    "copies": 123456,
    "colorConfiguration": "String",
  }
}

```
