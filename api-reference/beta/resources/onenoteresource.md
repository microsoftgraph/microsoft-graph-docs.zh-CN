---
title: onenoteResource 资源类型
description: 'OneNote 页面上的图像或其他文件资源。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 6e95775881ef78c70c50a634134ba20341173e77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039193"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="dd170-103">onenoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd170-103">onenoteResource resource type</span></span>

<span data-ttu-id="dd170-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd170-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd170-105">OneNote 页面上的图像或其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="dd170-105">An image or other file resource on a OneNote page.</span></span>

<span data-ttu-id="dd170-106">您可以获取资源的二进制数据，但不支持获取资源对象或资源集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd170-106">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": "String (Stream)",
  "contentUrl": "String"
}

```
<span data-ttu-id="dd170-107">通过向资源的终结点发送 GET 请求获取特定资源的二进制数据 `content` ：</span><span class="sxs-lookup"><span data-stu-id="dd170-107">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="dd170-108">当您使用以下请求获取页面的 HTML 内容时，将返回文件的资源 URI：</span><span class="sxs-lookup"><span data-stu-id="dd170-108">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="dd170-109">在页面 HTML 中， `img` 标记包含属性中的原始图像资源 `data-fullres-src` 和属性中优化的图像的终结点 `src` ：</span><span class="sxs-lookup"><span data-stu-id="dd170-109">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="dd170-110">一个 `object` 代表文件（如 PDF、.docx 和 PNG）的标记 () 在属性中包含文件资源的终结点 `data` ：</span><span class="sxs-lookup"><span data-stu-id="dd170-110">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="dd170-111">属性</span><span class="sxs-lookup"><span data-stu-id="dd170-111">Properties</span></span>
| <span data-ttu-id="dd170-112">属性</span><span class="sxs-lookup"><span data-stu-id="dd170-112">Property</span></span>     | <span data-ttu-id="dd170-113">类型</span><span class="sxs-lookup"><span data-stu-id="dd170-113">Type</span></span>   |<span data-ttu-id="dd170-114">说明</span><span class="sxs-lookup"><span data-stu-id="dd170-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd170-115">内容</span><span class="sxs-lookup"><span data-stu-id="dd170-115">content</span></span> | <span data-ttu-id="dd170-116">Edm</span><span class="sxs-lookup"><span data-stu-id="dd170-116">Edm.Stream</span></span>||
| <span data-ttu-id="dd170-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="dd170-117">contentUrl</span></span> | <span data-ttu-id="dd170-118">String</span><span class="sxs-lookup"><span data-stu-id="dd170-118">String</span></span> ||

## <a name="relationships"></a><span data-ttu-id="dd170-119">关系</span><span class="sxs-lookup"><span data-stu-id="dd170-119">Relationships</span></span>
<span data-ttu-id="dd170-120">无。</span><span class="sxs-lookup"><span data-stu-id="dd170-120">None.</span></span>


## <a name="methods"></a><span data-ttu-id="dd170-121">方法</span><span class="sxs-lookup"><span data-stu-id="dd170-121">Methods</span></span>
| <span data-ttu-id="dd170-122">方法</span><span class="sxs-lookup"><span data-stu-id="dd170-122">Method</span></span>           | <span data-ttu-id="dd170-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd170-123">Return Type</span></span>    |<span data-ttu-id="dd170-124">说明</span><span class="sxs-lookup"><span data-stu-id="dd170-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd170-125">获取资源二进制数据</span><span class="sxs-lookup"><span data-stu-id="dd170-125">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="dd170-126">Stream</span><span class="sxs-lookup"><span data-stu-id="dd170-126">Stream</span></span> |<span data-ttu-id="dd170-127">检索文件或图像资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="dd170-127">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


