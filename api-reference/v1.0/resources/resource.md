---
title: OneNoteResource 资源类型
description: 'OneNote 页面上的图像或其他文件资源。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 56004eafb469c15b735f2213d9ea18ee5bd17124
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806784"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="5f932-103">OneNoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f932-103">OneNoteResource resource type</span></span>

<span data-ttu-id="5f932-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f932-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f932-105">OneNote 页面上的图像或其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="5f932-105">An image or other file resource on a OneNote page.</span></span>

<span data-ttu-id="5f932-106">您可以获取资源的二进制数据，但不支持获取资源对象或资源集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f932-106">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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

<span data-ttu-id="5f932-107">通过向资源的终结点发送 GET 请求获取特定资源的二进制数据 `content` ：</span><span class="sxs-lookup"><span data-stu-id="5f932-107">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="5f932-108">当您使用以下请求获取页面的 HTML 内容时，将返回文件的资源 URI：</span><span class="sxs-lookup"><span data-stu-id="5f932-108">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="5f932-109">在页面 HTML 中， `img` 标记包含属性中的原始图像资源 `data-fullres-src` 和属性中优化的图像的终结点 `src` ：</span><span class="sxs-lookup"><span data-stu-id="5f932-109">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="5f932-110">一个 `object` 代表文件（如 PDF、.docx 和 PNG）的标记 () 在属性中包含文件资源的终结点 `data` ：</span><span class="sxs-lookup"><span data-stu-id="5f932-110">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="5f932-111">属性</span><span class="sxs-lookup"><span data-stu-id="5f932-111">Properties</span></span>

| <span data-ttu-id="5f932-112">属性</span><span class="sxs-lookup"><span data-stu-id="5f932-112">Property</span></span>             | <span data-ttu-id="5f932-113">类型</span><span class="sxs-lookup"><span data-stu-id="5f932-113">Type</span></span>            | <span data-ttu-id="5f932-114">说明</span><span class="sxs-lookup"><span data-stu-id="5f932-114">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="5f932-115">content</span><span class="sxs-lookup"><span data-stu-id="5f932-115">content</span></span>              | <span data-ttu-id="5f932-116">流</span><span class="sxs-lookup"><span data-stu-id="5f932-116">Stream</span></span>          | <span data-ttu-id="5f932-117">内容流</span><span class="sxs-lookup"><span data-stu-id="5f932-117">The content stream</span></span>
| <span data-ttu-id="5f932-118">contentUrl</span><span class="sxs-lookup"><span data-stu-id="5f932-118">contentUrl</span></span>           | <span data-ttu-id="5f932-119"> (url 的字符串) </span><span class="sxs-lookup"><span data-stu-id="5f932-119">String (url)</span></span>    | <span data-ttu-id="5f932-120">用于下载内容的 URL</span><span class="sxs-lookup"><span data-stu-id="5f932-120">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="5f932-121">关系</span><span class="sxs-lookup"><span data-stu-id="5f932-121">Relationships</span></span>
<span data-ttu-id="5f932-122">无。</span><span class="sxs-lookup"><span data-stu-id="5f932-122">None.</span></span>


## <a name="methods"></a><span data-ttu-id="5f932-123">方法</span><span class="sxs-lookup"><span data-stu-id="5f932-123">Methods</span></span>
| <span data-ttu-id="5f932-124">方法</span><span class="sxs-lookup"><span data-stu-id="5f932-124">Method</span></span>           | <span data-ttu-id="5f932-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f932-125">Return Type</span></span>    |<span data-ttu-id="5f932-126">说明</span><span class="sxs-lookup"><span data-stu-id="5f932-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f932-127">获取资源二进制数据</span><span class="sxs-lookup"><span data-stu-id="5f932-127">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="5f932-128">Stream</span><span class="sxs-lookup"><span data-stu-id="5f932-128">Stream</span></span> |<span data-ttu-id="5f932-129">检索文件或图像资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="5f932-129">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
