---
title: OneNoteResource 资源类型
description: 'OneNote 页面上的图像或其他文件资源。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: df3a11007de41b2ec503e8dd54cd6d0a1a7ee071
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967238"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="fc540-103">OneNoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc540-103">OneNoteResource resource type</span></span>

<span data-ttu-id="fc540-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc540-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc540-105">OneNote 页面上的图像或其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="fc540-105">An image or other file resource on a OneNote page.</span></span>

<span data-ttu-id="fc540-106">您可以获取资源的二进制数据，但不支持获取资源对象或资源集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc540-106">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="fc540-107">通过向资源的终结点发送 GET 请求获取特定资源的二进制数据 `content` ：</span><span class="sxs-lookup"><span data-stu-id="fc540-107">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="fc540-108">当您使用以下请求获取页面的 HTML 内容时，将返回文件的资源 URI：</span><span class="sxs-lookup"><span data-stu-id="fc540-108">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="fc540-109">在页面 HTML 中， `img` 标记包含属性中的原始图像资源 `data-fullres-src` 和属性中优化的图像的终结点 `src` ：</span><span class="sxs-lookup"><span data-stu-id="fc540-109">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="fc540-110">一个 `object` 代表文件（如 PDF、.docx 和 PNG）的标记 () 在属性中包含文件资源的终结点 `data` ：</span><span class="sxs-lookup"><span data-stu-id="fc540-110">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="fc540-111">属性</span><span class="sxs-lookup"><span data-stu-id="fc540-111">Properties</span></span>

| <span data-ttu-id="fc540-112">属性</span><span class="sxs-lookup"><span data-stu-id="fc540-112">Property</span></span>             | <span data-ttu-id="fc540-113">类型</span><span class="sxs-lookup"><span data-stu-id="fc540-113">Type</span></span>            | <span data-ttu-id="fc540-114">说明</span><span class="sxs-lookup"><span data-stu-id="fc540-114">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="fc540-115">content</span><span class="sxs-lookup"><span data-stu-id="fc540-115">content</span></span>              | <span data-ttu-id="fc540-116">流</span><span class="sxs-lookup"><span data-stu-id="fc540-116">Stream</span></span>          | <span data-ttu-id="fc540-117">内容流</span><span class="sxs-lookup"><span data-stu-id="fc540-117">The content stream</span></span>
| <span data-ttu-id="fc540-118">contentUrl</span><span class="sxs-lookup"><span data-stu-id="fc540-118">contentUrl</span></span>           | <span data-ttu-id="fc540-119"> (url 的字符串) </span><span class="sxs-lookup"><span data-stu-id="fc540-119">String (url)</span></span>    | <span data-ttu-id="fc540-120">用于下载内容的 URL</span><span class="sxs-lookup"><span data-stu-id="fc540-120">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="fc540-121">关系</span><span class="sxs-lookup"><span data-stu-id="fc540-121">Relationships</span></span>
<span data-ttu-id="fc540-122">无。</span><span class="sxs-lookup"><span data-stu-id="fc540-122">None.</span></span>


## <a name="methods"></a><span data-ttu-id="fc540-123">方法</span><span class="sxs-lookup"><span data-stu-id="fc540-123">Methods</span></span>
| <span data-ttu-id="fc540-124">方法</span><span class="sxs-lookup"><span data-stu-id="fc540-124">Method</span></span>           | <span data-ttu-id="fc540-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="fc540-125">Return Type</span></span>    |<span data-ttu-id="fc540-126">说明</span><span class="sxs-lookup"><span data-stu-id="fc540-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc540-127">获取资源二进制数据</span><span class="sxs-lookup"><span data-stu-id="fc540-127">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="fc540-128">Stream</span><span class="sxs-lookup"><span data-stu-id="fc540-128">Stream</span></span> |<span data-ttu-id="fc540-129">检索文件或图像资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="fc540-129">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

