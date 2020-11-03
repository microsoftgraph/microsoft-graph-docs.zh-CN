---
title: printDocument 资源类型
description: 代表要打印的文档。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c0bc886b618e061bee51ad82d7032737015f58ab
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849209"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="54de0-103">printDocument 资源类型</span><span class="sxs-lookup"><span data-stu-id="54de0-103">printDocument resource type</span></span>

<span data-ttu-id="54de0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54de0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54de0-105">代表要打印的文档。</span><span class="sxs-lookup"><span data-stu-id="54de0-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="54de0-106">方法</span><span class="sxs-lookup"><span data-stu-id="54de0-106">Methods</span></span>

| <span data-ttu-id="54de0-107">方法</span><span class="sxs-lookup"><span data-stu-id="54de0-107">Method</span></span>       | <span data-ttu-id="54de0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="54de0-108">Return Type</span></span> | <span data-ttu-id="54de0-109">说明</span><span class="sxs-lookup"><span data-stu-id="54de0-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="54de0-110">创建上传会话</span><span class="sxs-lookup"><span data-stu-id="54de0-110">Create upload session</span></span>](../api/printdocument-createuploadsession.md) | [<span data-ttu-id="54de0-111">uploadSession</span><span class="sxs-lookup"><span data-stu-id="54de0-111">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="54de0-112">创建一个上载会话，以以迭代方式上载 **printDocument** 的二进制文件的范围。</span><span class="sxs-lookup"><span data-stu-id="54de0-112">Create an upload session to iteratively upload ranges of binary file of the **printDocument**.</span></span> |
| [<span data-ttu-id="54de0-113">下载二进制文件</span><span class="sxs-lookup"><span data-stu-id="54de0-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="54de0-114">下载 Url</span><span class="sxs-lookup"><span data-stu-id="54de0-114">Download Url</span></span> | <span data-ttu-id="54de0-115">下载与 **printDocument** 相关联的二进制文件。</span><span class="sxs-lookup"><span data-stu-id="54de0-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="54de0-116">属性</span><span class="sxs-lookup"><span data-stu-id="54de0-116">Properties</span></span>
| <span data-ttu-id="54de0-117">属性</span><span class="sxs-lookup"><span data-stu-id="54de0-117">Property</span></span>     | <span data-ttu-id="54de0-118">类型</span><span class="sxs-lookup"><span data-stu-id="54de0-118">Type</span></span>        | <span data-ttu-id="54de0-119">说明</span><span class="sxs-lookup"><span data-stu-id="54de0-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54de0-120">id</span><span class="sxs-lookup"><span data-stu-id="54de0-120">id</span></span>|<span data-ttu-id="54de0-121">String</span><span class="sxs-lookup"><span data-stu-id="54de0-121">String</span></span>|<span data-ttu-id="54de0-122">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="54de0-122">The document's identifier.</span></span> <span data-ttu-id="54de0-123">只读。</span><span class="sxs-lookup"><span data-stu-id="54de0-123">Read-only.</span></span>|
|<span data-ttu-id="54de0-124">displayName</span><span class="sxs-lookup"><span data-stu-id="54de0-124">displayName</span></span>|<span data-ttu-id="54de0-125">String</span><span class="sxs-lookup"><span data-stu-id="54de0-125">String</span></span>|<span data-ttu-id="54de0-126">文档的名称。</span><span class="sxs-lookup"><span data-stu-id="54de0-126">The document's name.</span></span> <span data-ttu-id="54de0-127">只读。</span><span class="sxs-lookup"><span data-stu-id="54de0-127">Read-only.</span></span>|
|<span data-ttu-id="54de0-128">contentType</span><span class="sxs-lookup"><span data-stu-id="54de0-128">contentType</span></span>|<span data-ttu-id="54de0-129">String</span><span class="sxs-lookup"><span data-stu-id="54de0-129">String</span></span>|<span data-ttu-id="54de0-130">文档的内容 (MIME) 类型。</span><span class="sxs-lookup"><span data-stu-id="54de0-130">The document's content (MIME) type.</span></span> <span data-ttu-id="54de0-131">只读。</span><span class="sxs-lookup"><span data-stu-id="54de0-131">Read-only.</span></span>|
|<span data-ttu-id="54de0-132">size</span><span class="sxs-lookup"><span data-stu-id="54de0-132">size</span></span>|<span data-ttu-id="54de0-133">Int64</span><span class="sxs-lookup"><span data-stu-id="54de0-133">Int64</span></span>|<span data-ttu-id="54de0-134">文档的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="54de0-134">The document's size in bytes.</span></span> <span data-ttu-id="54de0-135">只读。</span><span class="sxs-lookup"><span data-stu-id="54de0-135">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54de0-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54de0-136">JSON representation</span></span>

<span data-ttu-id="54de0-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54de0-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": 12345
}

```


