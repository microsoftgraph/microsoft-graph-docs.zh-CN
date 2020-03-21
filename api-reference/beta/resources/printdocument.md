---
title: printDocument 资源类型
description: 代表要打印的文档。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2a981fbdf7e1126783ae97d93c20e3ec08b1f2f0
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895631"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="44143-103">printDocument 资源类型</span><span class="sxs-lookup"><span data-stu-id="44143-103">printDocument resource type</span></span>

<span data-ttu-id="44143-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44143-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44143-105">代表要打印的文档。</span><span class="sxs-lookup"><span data-stu-id="44143-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="44143-106">方法</span><span class="sxs-lookup"><span data-stu-id="44143-106">Methods</span></span>

| <span data-ttu-id="44143-107">方法</span><span class="sxs-lookup"><span data-stu-id="44143-107">Method</span></span>       | <span data-ttu-id="44143-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="44143-108">Return Type</span></span> | <span data-ttu-id="44143-109">说明</span><span class="sxs-lookup"><span data-stu-id="44143-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="44143-110">uploadData</span><span class="sxs-lookup"><span data-stu-id="44143-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="44143-111">无</span><span class="sxs-lookup"><span data-stu-id="44143-111">None</span></span> | <span data-ttu-id="44143-112">上载**printDocument**的单个二进制段。</span><span class="sxs-lookup"><span data-stu-id="44143-112">Upload a single binary segment of the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="44143-113">属性</span><span class="sxs-lookup"><span data-stu-id="44143-113">Properties</span></span>
| <span data-ttu-id="44143-114">属性</span><span class="sxs-lookup"><span data-stu-id="44143-114">Property</span></span>     | <span data-ttu-id="44143-115">类型</span><span class="sxs-lookup"><span data-stu-id="44143-115">Type</span></span>        | <span data-ttu-id="44143-116">说明</span><span class="sxs-lookup"><span data-stu-id="44143-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="44143-117">id</span><span class="sxs-lookup"><span data-stu-id="44143-117">id</span></span>|<span data-ttu-id="44143-118">String</span><span class="sxs-lookup"><span data-stu-id="44143-118">String</span></span>|<span data-ttu-id="44143-119">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="44143-119">The document's identifier.</span></span> <span data-ttu-id="44143-120">只读。</span><span class="sxs-lookup"><span data-stu-id="44143-120">Read-only.</span></span>|
|<span data-ttu-id="44143-121">name</span><span class="sxs-lookup"><span data-stu-id="44143-121">name</span></span>|<span data-ttu-id="44143-122">String</span><span class="sxs-lookup"><span data-stu-id="44143-122">String</span></span>|<span data-ttu-id="44143-123">文档的名称。</span><span class="sxs-lookup"><span data-stu-id="44143-123">The document's name.</span></span> <span data-ttu-id="44143-124">只读。</span><span class="sxs-lookup"><span data-stu-id="44143-124">Read-only.</span></span>|
|<span data-ttu-id="44143-125">mimeType</span><span class="sxs-lookup"><span data-stu-id="44143-125">mimeType</span></span>|<span data-ttu-id="44143-126">String</span><span class="sxs-lookup"><span data-stu-id="44143-126">String</span></span>|<span data-ttu-id="44143-127">文档的 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="44143-127">The document's MIME type.</span></span> <span data-ttu-id="44143-128">只读。</span><span class="sxs-lookup"><span data-stu-id="44143-128">Read-only.</span></span>|
|<span data-ttu-id="44143-129">sizeInBytes</span><span class="sxs-lookup"><span data-stu-id="44143-129">sizeInBytes</span></span>|<span data-ttu-id="44143-130">Int64</span><span class="sxs-lookup"><span data-stu-id="44143-130">Int64</span></span>|<span data-ttu-id="44143-131">文档的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="44143-131">The document's size in bytes.</span></span> <span data-ttu-id="44143-132">只读。</span><span class="sxs-lookup"><span data-stu-id="44143-132">Read-only.</span></span>|
|<span data-ttu-id="44143-133">documentConfiguration</span><span class="sxs-lookup"><span data-stu-id="44143-133">documentConfiguration</span></span>|[<span data-ttu-id="44143-134">printerDocumentConfiguration</span><span class="sxs-lookup"><span data-stu-id="44143-134">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="44143-135">打印机打印文档时应使用的一组设置。</span><span class="sxs-lookup"><span data-stu-id="44143-135">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="44143-136">只读。</span><span class="sxs-lookup"><span data-stu-id="44143-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44143-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44143-137">JSON representation</span></span>

<span data-ttu-id="44143-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44143-138">The following is a JSON representation of the resource.</span></span>

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
