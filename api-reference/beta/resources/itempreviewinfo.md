---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
ms.openlocfilehash: 469679e9baa016560f5a02425bc41d628a24dc2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509761"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="4018f-102">ItemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="4018f-102">ItemPreviewInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4018f-103">**ItemPreviewInfo**资源包含有关如何将嵌入的[DriveItem](driveitem.md)预览信息。</span><span class="sxs-lookup"><span data-stu-id="4018f-103">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4018f-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4018f-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="4018f-105">属性</span><span class="sxs-lookup"><span data-stu-id="4018f-105">Properties</span></span>

| <span data-ttu-id="4018f-106">名称</span><span class="sxs-lookup"><span data-stu-id="4018f-106">Name</span></span>           | <span data-ttu-id="4018f-107">类型</span><span class="sxs-lookup"><span data-stu-id="4018f-107">Type</span></span>   | <span data-ttu-id="4018f-108">说明</span><span class="sxs-lookup"><span data-stu-id="4018f-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="4018f-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="4018f-109">getUrl</span></span>         | <span data-ttu-id="4018f-110">string</span><span class="sxs-lookup"><span data-stu-id="4018f-110">string</span></span> | <span data-ttu-id="4018f-111">适用于嵌入使用 HTTP GET （iframe 等） 的 URL</span><span class="sxs-lookup"><span data-stu-id="4018f-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="4018f-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="4018f-112">postUrl</span></span>        | <span data-ttu-id="4018f-113">string</span><span class="sxs-lookup"><span data-stu-id="4018f-113">string</span></span> | <span data-ttu-id="4018f-114">适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）</span><span class="sxs-lookup"><span data-stu-id="4018f-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="4018f-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="4018f-115">postParameters</span></span> | <span data-ttu-id="4018f-116">string</span><span class="sxs-lookup"><span data-stu-id="4018f-116">string</span></span> | <span data-ttu-id="4018f-117">如果使用 postUrl 包括 POST 参数</span><span class="sxs-lookup"><span data-stu-id="4018f-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="4018f-118">GetUrl、 postUrl，或同时可能会返回根据支持指定的选项的当前状态。</span><span class="sxs-lookup"><span data-stu-id="4018f-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="4018f-119">postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。</span><span class="sxs-lookup"><span data-stu-id="4018f-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="4018f-120">例如：</span><span class="sxs-lookup"><span data-stu-id="4018f-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="4018f-121">不透明应考虑的 Url 和参数的格式。</span><span class="sxs-lookup"><span data-stu-id="4018f-121">The formats of URLs and parameters should be considered opaque.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/itempreviewinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
