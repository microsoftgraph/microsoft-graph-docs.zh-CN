---
title: onenoteResource 资源类型
description: 'OneNote 页面上的图像或其他文件资源。 '
localization_priority: Normal
ms.openlocfilehash: abb60a52b0f32ac2e1bdc024d07f02233db6043c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348570"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="e6030-103">onenoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6030-103">onenoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6030-104">OneNote 页面上的图像或其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="e6030-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="e6030-105">您可以获取资源的二进制数据, 但不支持获取资源对象或资源集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6030-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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
<span data-ttu-id="e6030-106">通过向资源的`content`终结点发送 get 请求获取特定资源的二进制数据:</span><span class="sxs-lookup"><span data-stu-id="e6030-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="e6030-107">当您使用以下请求获取页面的 HTML 内容时, 将返回文件的资源 URI:</span><span class="sxs-lookup"><span data-stu-id="e6030-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="e6030-108">在页面 HTML 中, `img`标记包含`data-fullres-src`属性中的原始图像资源和`src`属性中优化的图像的终结点:</span><span class="sxs-lookup"><span data-stu-id="e6030-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="e6030-109">`object`标记 (表示 PDF、.docx 和 PNG 等文件) 包含`data`属性中的文件资源的终结点:</span><span class="sxs-lookup"><span data-stu-id="e6030-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="e6030-110">属性</span><span class="sxs-lookup"><span data-stu-id="e6030-110">Properties</span></span>
| <span data-ttu-id="e6030-111">属性</span><span class="sxs-lookup"><span data-stu-id="e6030-111">Property</span></span>     | <span data-ttu-id="e6030-112">类型</span><span class="sxs-lookup"><span data-stu-id="e6030-112">Type</span></span>   |<span data-ttu-id="e6030-113">说明</span><span class="sxs-lookup"><span data-stu-id="e6030-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6030-114">内容</span><span class="sxs-lookup"><span data-stu-id="e6030-114">content</span></span> | <span data-ttu-id="e6030-115">Edm</span><span class="sxs-lookup"><span data-stu-id="e6030-115">Edm.Stream</span></span>||
| <span data-ttu-id="e6030-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="e6030-116">contentUrl</span></span> | <span data-ttu-id="e6030-117">String</span><span class="sxs-lookup"><span data-stu-id="e6030-117">String</span></span> ||

## <a name="relationships"></a><span data-ttu-id="e6030-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="e6030-118">Relationships</span></span>
<span data-ttu-id="e6030-119">无。</span><span class="sxs-lookup"><span data-stu-id="e6030-119">None.</span></span>


## <a name="methods"></a><span data-ttu-id="e6030-120">方法</span><span class="sxs-lookup"><span data-stu-id="e6030-120">Methods</span></span>
| <span data-ttu-id="e6030-121">方法</span><span class="sxs-lookup"><span data-stu-id="e6030-121">Method</span></span>           | <span data-ttu-id="e6030-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="e6030-122">Return Type</span></span>    |<span data-ttu-id="e6030-123">说明</span><span class="sxs-lookup"><span data-stu-id="e6030-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6030-124">获取资源二进制数据</span><span class="sxs-lookup"><span data-stu-id="e6030-124">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="e6030-125">流</span><span class="sxs-lookup"><span data-stu-id="e6030-125">Stream</span></span> |<span data-ttu-id="e6030-126">检索文件或图像资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="e6030-126">Retrieve the binary data of a file or image resource.</span></span>|

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
