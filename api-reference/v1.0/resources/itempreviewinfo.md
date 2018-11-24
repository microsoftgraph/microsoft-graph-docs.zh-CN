---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: ebac77d2ca32438e552831de0258fe5e86fa225a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2018
ms.locfileid: "26605975"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="a47e0-102">itemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a47e0-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="a47e0-103">**ItemPreviewInfo**资源包含有关如何将嵌入的[driveItem](driveitem.md)预览信息。</span><span class="sxs-lookup"><span data-stu-id="a47e0-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a47e0-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a47e0-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="a47e0-105">属性</span><span class="sxs-lookup"><span data-stu-id="a47e0-105">Properties</span></span>

| <span data-ttu-id="a47e0-106">名称</span><span class="sxs-lookup"><span data-stu-id="a47e0-106">Name</span></span>           | <span data-ttu-id="a47e0-107">类型</span><span class="sxs-lookup"><span data-stu-id="a47e0-107">Type</span></span>   | <span data-ttu-id="a47e0-108">说明</span><span class="sxs-lookup"><span data-stu-id="a47e0-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="a47e0-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="a47e0-109">getUrl</span></span>         | <span data-ttu-id="a47e0-110">string</span><span class="sxs-lookup"><span data-stu-id="a47e0-110">string</span></span> | <span data-ttu-id="a47e0-111">适用于嵌入使用 HTTP GET （iframe 等） 的 URL</span><span class="sxs-lookup"><span data-stu-id="a47e0-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="a47e0-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="a47e0-112">postUrl</span></span>        | <span data-ttu-id="a47e0-113">string</span><span class="sxs-lookup"><span data-stu-id="a47e0-113">string</span></span> | <span data-ttu-id="a47e0-114">适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）</span><span class="sxs-lookup"><span data-stu-id="a47e0-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="a47e0-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="a47e0-115">postParameters</span></span> | <span data-ttu-id="a47e0-116">string</span><span class="sxs-lookup"><span data-stu-id="a47e0-116">string</span></span> | <span data-ttu-id="a47e0-117">如果使用 postUrl 包括 POST 参数</span><span class="sxs-lookup"><span data-stu-id="a47e0-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="a47e0-118">GetUrl、 postUrl，或同时可能会返回根据支持指定的选项的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a47e0-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="a47e0-119">postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。</span><span class="sxs-lookup"><span data-stu-id="a47e0-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="a47e0-120">例如：</span><span class="sxs-lookup"><span data-stu-id="a47e0-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="a47e0-121">不透明应考虑的 Url 和参数的格式。</span><span class="sxs-lookup"><span data-stu-id="a47e0-121">The formats of URLs and parameters should be considered opaque.</span></span>
