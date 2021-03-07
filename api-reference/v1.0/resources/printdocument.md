---
title: printDocument 资源类型
description: 表示正在打印的文档。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d8ca73a6e8acfb6ac2326b171b2b8c04fed7e039
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517196"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="736a4-103">printDocument 资源类型</span><span class="sxs-lookup"><span data-stu-id="736a4-103">printDocument resource type</span></span>

<span data-ttu-id="736a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="736a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="736a4-105">表示正在打印的文档。</span><span class="sxs-lookup"><span data-stu-id="736a4-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="736a4-106">Methods</span><span class="sxs-lookup"><span data-stu-id="736a4-106">Methods</span></span>
|<span data-ttu-id="736a4-107">方法</span><span class="sxs-lookup"><span data-stu-id="736a4-107">Method</span></span>|<span data-ttu-id="736a4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="736a4-108">Return type</span></span>|<span data-ttu-id="736a4-109">Description</span><span class="sxs-lookup"><span data-stu-id="736a4-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="736a4-110">创建上载会话</span><span class="sxs-lookup"><span data-stu-id="736a4-110">Create upload session</span></span>](../api/printdocument-createuploadsession.md) | [<span data-ttu-id="736a4-111">uploadSession</span><span class="sxs-lookup"><span data-stu-id="736a4-111">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="736a4-112">创建上载会话以迭代上载 **printDocument** 的二进制文件范围。</span><span class="sxs-lookup"><span data-stu-id="736a4-112">Create an upload session to iteratively upload ranges of binary file of the **printDocument**.</span></span> |
| [<span data-ttu-id="736a4-113">下载二进制文件</span><span class="sxs-lookup"><span data-stu-id="736a4-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="736a4-114">下载 Url</span><span class="sxs-lookup"><span data-stu-id="736a4-114">Download Url</span></span> | <span data-ttu-id="736a4-115">下载与 **printDocument 关联的二进制文件**。</span><span class="sxs-lookup"><span data-stu-id="736a4-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="736a4-116">属性</span><span class="sxs-lookup"><span data-stu-id="736a4-116">Properties</span></span>
|<span data-ttu-id="736a4-117">属性</span><span class="sxs-lookup"><span data-stu-id="736a4-117">Property</span></span>|<span data-ttu-id="736a4-118">类型</span><span class="sxs-lookup"><span data-stu-id="736a4-118">Type</span></span>|<span data-ttu-id="736a4-119">说明</span><span class="sxs-lookup"><span data-stu-id="736a4-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="736a4-120">id</span><span class="sxs-lookup"><span data-stu-id="736a4-120">id</span></span>|<span data-ttu-id="736a4-121">String</span><span class="sxs-lookup"><span data-stu-id="736a4-121">String</span></span>|<span data-ttu-id="736a4-122">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="736a4-122">The document's identifier.</span></span> <span data-ttu-id="736a4-123">只读。</span><span class="sxs-lookup"><span data-stu-id="736a4-123">Read-only.</span></span>|
|<span data-ttu-id="736a4-124">displayName</span><span class="sxs-lookup"><span data-stu-id="736a4-124">displayName</span></span>|<span data-ttu-id="736a4-125">String</span><span class="sxs-lookup"><span data-stu-id="736a4-125">String</span></span>|<span data-ttu-id="736a4-126">文档的名称。</span><span class="sxs-lookup"><span data-stu-id="736a4-126">The document's name.</span></span> <span data-ttu-id="736a4-127">只读。</span><span class="sxs-lookup"><span data-stu-id="736a4-127">Read-only.</span></span>|
|<span data-ttu-id="736a4-128">contentType</span><span class="sxs-lookup"><span data-stu-id="736a4-128">contentType</span></span>|<span data-ttu-id="736a4-129">String</span><span class="sxs-lookup"><span data-stu-id="736a4-129">String</span></span>|<span data-ttu-id="736a4-130">文档的内容类型 (MIME) 类型。</span><span class="sxs-lookup"><span data-stu-id="736a4-130">The document's content (MIME) type.</span></span> <span data-ttu-id="736a4-131">只读。</span><span class="sxs-lookup"><span data-stu-id="736a4-131">Read-only.</span></span>|
|<span data-ttu-id="736a4-132">size</span><span class="sxs-lookup"><span data-stu-id="736a4-132">size</span></span>|<span data-ttu-id="736a4-133">Int64</span><span class="sxs-lookup"><span data-stu-id="736a4-133">Int64</span></span>|<span data-ttu-id="736a4-134">文档的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="736a4-134">The document's size in bytes.</span></span> <span data-ttu-id="736a4-135">只读。</span><span class="sxs-lookup"><span data-stu-id="736a4-135">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="736a4-136">关系</span><span class="sxs-lookup"><span data-stu-id="736a4-136">Relationships</span></span>
<span data-ttu-id="736a4-137">无。</span><span class="sxs-lookup"><span data-stu-id="736a4-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="736a4-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="736a4-138">JSON representation</span></span>
<span data-ttu-id="736a4-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="736a4-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printDocument",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": "Integer"
}
```