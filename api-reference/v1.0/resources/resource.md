---
title: OneNoteResource 资源类型
description: 'OneNote 页面上的图像或其他文件资源。 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 03dde18905892538e4f883f2e90b6b0c36fda460
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446973"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="9db00-103">OneNoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="9db00-103">OneNoteResource resource type</span></span>

<span data-ttu-id="9db00-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9db00-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9db00-105">OneNote 页面上的图像或其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="9db00-105">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="9db00-106">您可以获取资源的二进制数据，但不支持获取资源对象或资源集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9db00-106">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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

<span data-ttu-id="9db00-107">通过向资源的`content`终结点发送 get 请求获取特定资源的二进制数据：</span><span class="sxs-lookup"><span data-stu-id="9db00-107">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="9db00-108">当您使用以下请求获取页面的 HTML 内容时，将返回文件的资源 URI：</span><span class="sxs-lookup"><span data-stu-id="9db00-108">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="9db00-109">在页面 HTML 中， `img`标记包含`data-fullres-src`属性中的原始图像资源和`src`属性中优化的图像的终结点：</span><span class="sxs-lookup"><span data-stu-id="9db00-109">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="9db00-110">`object`标记（表示 PDF、.DOCX 和 PNG 等文件）包含`data`属性中的文件资源的终结点：</span><span class="sxs-lookup"><span data-stu-id="9db00-110">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="9db00-111">属性</span><span class="sxs-lookup"><span data-stu-id="9db00-111">Properties</span></span>

| <span data-ttu-id="9db00-112">属性</span><span class="sxs-lookup"><span data-stu-id="9db00-112">Property</span></span>             | <span data-ttu-id="9db00-113">类型</span><span class="sxs-lookup"><span data-stu-id="9db00-113">Type</span></span>            | <span data-ttu-id="9db00-114">说明</span><span class="sxs-lookup"><span data-stu-id="9db00-114">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="9db00-115">content</span><span class="sxs-lookup"><span data-stu-id="9db00-115">content</span></span>              | <span data-ttu-id="9db00-116">流</span><span class="sxs-lookup"><span data-stu-id="9db00-116">Stream</span></span>          | <span data-ttu-id="9db00-117">内容流</span><span class="sxs-lookup"><span data-stu-id="9db00-117">The content stream</span></span>
| <span data-ttu-id="9db00-118">contentUrl</span><span class="sxs-lookup"><span data-stu-id="9db00-118">contentUrl</span></span>           | <span data-ttu-id="9db00-119">String （url）</span><span class="sxs-lookup"><span data-stu-id="9db00-119">String (url)</span></span>    | <span data-ttu-id="9db00-120">用于下载内容的 URL</span><span class="sxs-lookup"><span data-stu-id="9db00-120">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="9db00-121">关系</span><span class="sxs-lookup"><span data-stu-id="9db00-121">Relationships</span></span>
<span data-ttu-id="9db00-122">无。</span><span class="sxs-lookup"><span data-stu-id="9db00-122">None.</span></span>


## <a name="methods"></a><span data-ttu-id="9db00-123">方法</span><span class="sxs-lookup"><span data-stu-id="9db00-123">Methods</span></span>
| <span data-ttu-id="9db00-124">方法</span><span class="sxs-lookup"><span data-stu-id="9db00-124">Method</span></span>           | <span data-ttu-id="9db00-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="9db00-125">Return Type</span></span>    |<span data-ttu-id="9db00-126">说明</span><span class="sxs-lookup"><span data-stu-id="9db00-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9db00-127">获取资源二进制数据</span><span class="sxs-lookup"><span data-stu-id="9db00-127">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="9db00-128">Stream</span><span class="sxs-lookup"><span data-stu-id="9db00-128">Stream</span></span> |<span data-ttu-id="9db00-129">检索文件或图像资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="9db00-129">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
