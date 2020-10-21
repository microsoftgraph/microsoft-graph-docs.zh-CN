---
title: printDocument 资源类型
description: 代表要打印的文档。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 34f35181e9d1ba70c2efe8df31d6d6457aa0acde
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635136"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="6bef9-103">printDocument 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bef9-103">printDocument resource type</span></span>

<span data-ttu-id="6bef9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bef9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bef9-105">代表要打印的文档。</span><span class="sxs-lookup"><span data-stu-id="6bef9-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="6bef9-106">方法</span><span class="sxs-lookup"><span data-stu-id="6bef9-106">Methods</span></span>

| <span data-ttu-id="6bef9-107">方法</span><span class="sxs-lookup"><span data-stu-id="6bef9-107">Method</span></span>       | <span data-ttu-id="6bef9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6bef9-108">Return Type</span></span> | <span data-ttu-id="6bef9-109">说明</span><span class="sxs-lookup"><span data-stu-id="6bef9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6bef9-110">uploadData</span><span class="sxs-lookup"><span data-stu-id="6bef9-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="6bef9-111">无</span><span class="sxs-lookup"><span data-stu-id="6bef9-111">None</span></span> | <span data-ttu-id="6bef9-112">上载 **printDocument**的单个二进制段。</span><span class="sxs-lookup"><span data-stu-id="6bef9-112">Upload a single binary segment of the **printDocument**.</span></span> |
| [<span data-ttu-id="6bef9-113">下载二进制文件</span><span class="sxs-lookup"><span data-stu-id="6bef9-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="6bef9-114">下载 Url</span><span class="sxs-lookup"><span data-stu-id="6bef9-114">Download Url</span></span> | <span data-ttu-id="6bef9-115">下载与 **printDocument**相关联的二进制文件。</span><span class="sxs-lookup"><span data-stu-id="6bef9-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="6bef9-116">属性</span><span class="sxs-lookup"><span data-stu-id="6bef9-116">Properties</span></span>
| <span data-ttu-id="6bef9-117">属性</span><span class="sxs-lookup"><span data-stu-id="6bef9-117">Property</span></span>     | <span data-ttu-id="6bef9-118">类型</span><span class="sxs-lookup"><span data-stu-id="6bef9-118">Type</span></span>        | <span data-ttu-id="6bef9-119">说明</span><span class="sxs-lookup"><span data-stu-id="6bef9-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6bef9-120">id</span><span class="sxs-lookup"><span data-stu-id="6bef9-120">id</span></span>|<span data-ttu-id="6bef9-121">String</span><span class="sxs-lookup"><span data-stu-id="6bef9-121">String</span></span>|<span data-ttu-id="6bef9-122">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="6bef9-122">The document's identifier.</span></span> <span data-ttu-id="6bef9-123">只读。</span><span class="sxs-lookup"><span data-stu-id="6bef9-123">Read-only.</span></span>|
|<span data-ttu-id="6bef9-124">displayName</span><span class="sxs-lookup"><span data-stu-id="6bef9-124">displayName</span></span>|<span data-ttu-id="6bef9-125">String</span><span class="sxs-lookup"><span data-stu-id="6bef9-125">String</span></span>|<span data-ttu-id="6bef9-126">文档的名称。</span><span class="sxs-lookup"><span data-stu-id="6bef9-126">The document's name.</span></span> <span data-ttu-id="6bef9-127">只读。</span><span class="sxs-lookup"><span data-stu-id="6bef9-127">Read-only.</span></span>|
|<span data-ttu-id="6bef9-128">contentType</span><span class="sxs-lookup"><span data-stu-id="6bef9-128">contentType</span></span>|<span data-ttu-id="6bef9-129">String</span><span class="sxs-lookup"><span data-stu-id="6bef9-129">String</span></span>|<span data-ttu-id="6bef9-130">文档的内容 (MIME) 类型。</span><span class="sxs-lookup"><span data-stu-id="6bef9-130">The document's content (MIME) type.</span></span> <span data-ttu-id="6bef9-131">只读。</span><span class="sxs-lookup"><span data-stu-id="6bef9-131">Read-only.</span></span>|
|<span data-ttu-id="6bef9-132">size</span><span class="sxs-lookup"><span data-stu-id="6bef9-132">size</span></span>|<span data-ttu-id="6bef9-133">Int64</span><span class="sxs-lookup"><span data-stu-id="6bef9-133">Int64</span></span>|<span data-ttu-id="6bef9-134">文档的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="6bef9-134">The document's size in bytes.</span></span> <span data-ttu-id="6bef9-135">只读。</span><span class="sxs-lookup"><span data-stu-id="6bef9-135">Read-only.</span></span>|
|<span data-ttu-id="6bef9-136">configuration</span><span class="sxs-lookup"><span data-stu-id="6bef9-136">configuration</span></span>|[<span data-ttu-id="6bef9-137">printerDocumentConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bef9-137">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="6bef9-138">打印机打印文档时应使用的一组设置。</span><span class="sxs-lookup"><span data-stu-id="6bef9-138">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="6bef9-139">只读。</span><span class="sxs-lookup"><span data-stu-id="6bef9-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bef9-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bef9-140">JSON representation</span></span>

<span data-ttu-id="6bef9-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bef9-141">The following is a JSON representation of the resource.</span></span>

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
    "colorConfiguration": "String"
  }
}

```


