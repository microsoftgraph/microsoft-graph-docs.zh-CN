---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
ms.openlocfilehash: 469679e9baa016560f5a02425bc41d628a24dc2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562865"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="c6a19-102">ItemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6a19-102">ItemPreviewInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6a19-103">**ItemPreviewInfo**资源包含有关如何嵌入[DriveItem](driveitem.md)的预览的信息。</span><span class="sxs-lookup"><span data-stu-id="c6a19-103">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6a19-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6a19-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="c6a19-105">属性</span><span class="sxs-lookup"><span data-stu-id="c6a19-105">Properties</span></span>

| <span data-ttu-id="c6a19-106">名称</span><span class="sxs-lookup"><span data-stu-id="c6a19-106">Name</span></span>           | <span data-ttu-id="c6a19-107">类型</span><span class="sxs-lookup"><span data-stu-id="c6a19-107">Type</span></span>   | <span data-ttu-id="c6a19-108">说明</span><span class="sxs-lookup"><span data-stu-id="c6a19-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="c6a19-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="c6a19-109">getUrl</span></span>         | <span data-ttu-id="c6a19-110">string</span><span class="sxs-lookup"><span data-stu-id="c6a19-110">string</span></span> | <span data-ttu-id="c6a19-111">适合使用 HTTP GET (iframe 等) 进行嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="c6a19-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="c6a19-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="c6a19-112">postUrl</span></span>        | <span data-ttu-id="c6a19-113">string</span><span class="sxs-lookup"><span data-stu-id="c6a19-113">string</span></span> | <span data-ttu-id="c6a19-114">适合使用 HTTP POST (窗体 POST、JS 等) 嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="c6a19-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="c6a19-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="c6a19-115">postParameters</span></span> | <span data-ttu-id="c6a19-116">string</span><span class="sxs-lookup"><span data-stu-id="c6a19-116">string</span></span> | <span data-ttu-id="c6a19-117">如果使用 postUrl, 则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="c6a19-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="c6a19-118">根据指定选项的当前支持状态, 可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="c6a19-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="c6a19-119">postParameters 是格式为`application/x-www-form-urlencoded`的字符串, 如果向 postUrl 执行 POST, 应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="c6a19-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="c6a19-120">例如：</span><span class="sxs-lookup"><span data-stu-id="c6a19-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="c6a19-121">url 和参数的格式应被认为是不透明的。</span><span class="sxs-lookup"><span data-stu-id="c6a19-121">The formats of URLs and parameters should be considered opaque.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/itempreviewinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
