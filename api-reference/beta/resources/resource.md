---
title: 资源资源类型
description: 'OneNote 页面上的图像或其他文件资源。 '
localization_priority: Normal
ms.openlocfilehash: c85897af91290df83f4d6fccaf0552513b4f0535
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563015"
---
# <a name="resource-resource-type"></a><span data-ttu-id="e58e7-103">资源资源类型</span><span class="sxs-lookup"><span data-stu-id="e58e7-103">resource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e58e7-104">OneNote 页面上的图像或其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="e58e7-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="e58e7-105">您可以获取资源的二进制数据, 但不支持获取资源对象或资源集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e58e7-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="e58e7-106">通过向资源的`content`终结点发送 get 请求获取特定资源的二进制数据:</span><span class="sxs-lookup"><span data-stu-id="e58e7-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="e58e7-107">当您使用以下请求获取页面的 HTML 内容时, 将返回文件的资源 URI:</span><span class="sxs-lookup"><span data-stu-id="e58e7-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="e58e7-108">在页面 HTML 中, `img`标记包含`data-fullres-src`属性中的原始图像资源和`src`属性中优化的图像的终结点:</span><span class="sxs-lookup"><span data-stu-id="e58e7-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="e58e7-109">`object`标记 (表示 PDF、.docx 和 PNG 等文件) 包含`data`属性中的文件资源的终结点:</span><span class="sxs-lookup"><span data-stu-id="e58e7-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="e58e7-110">属性</span><span class="sxs-lookup"><span data-stu-id="e58e7-110">Properties</span></span>
<span data-ttu-id="e58e7-111">表示组件的一个实例，这是运行时对用户的指定组件的实例化。对象包含实验室特定运行的组件的已翻译视图。</span><span class="sxs-lookup"><span data-stu-id="e58e7-111">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e58e7-112">关系</span><span class="sxs-lookup"><span data-stu-id="e58e7-112">Relationships</span></span>
<span data-ttu-id="e58e7-113">无。</span><span class="sxs-lookup"><span data-stu-id="e58e7-113">None.</span></span>


## <a name="methods"></a><span data-ttu-id="e58e7-114">方法</span><span class="sxs-lookup"><span data-stu-id="e58e7-114">Methods</span></span>
| <span data-ttu-id="e58e7-115">方法</span><span class="sxs-lookup"><span data-stu-id="e58e7-115">Method</span></span>           | <span data-ttu-id="e58e7-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="e58e7-116">Return Type</span></span>    |<span data-ttu-id="e58e7-117">说明</span><span class="sxs-lookup"><span data-stu-id="e58e7-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e58e7-118">获取资源二进制数据</span><span class="sxs-lookup"><span data-stu-id="e58e7-118">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="e58e7-119">Stream</span><span class="sxs-lookup"><span data-stu-id="e58e7-119">Stream</span></span> |<span data-ttu-id="e58e7-120">检索文件或图像资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="e58e7-120">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
