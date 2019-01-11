---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
ms.openlocfilehash: 0f2a161b9b43a8d372b90530b1b9d9244f77d8e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857342"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="fd212-102">ItemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd212-102">ItemPreviewInfo resource type</span></span>

> <span data-ttu-id="fd212-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fd212-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd212-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fd212-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd212-105">**ItemPreviewInfo**资源包含有关如何将嵌入的[DriveItem](driveitem.md)预览信息。</span><span class="sxs-lookup"><span data-stu-id="fd212-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd212-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd212-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="fd212-107">属性</span><span class="sxs-lookup"><span data-stu-id="fd212-107">Properties</span></span>

| <span data-ttu-id="fd212-108">名称</span><span class="sxs-lookup"><span data-stu-id="fd212-108">Name</span></span>           | <span data-ttu-id="fd212-109">类型</span><span class="sxs-lookup"><span data-stu-id="fd212-109">Type</span></span>   | <span data-ttu-id="fd212-110">Description</span><span class="sxs-lookup"><span data-stu-id="fd212-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="fd212-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="fd212-111">getUrl</span></span>         | <span data-ttu-id="fd212-112">string</span><span class="sxs-lookup"><span data-stu-id="fd212-112">string</span></span> | <span data-ttu-id="fd212-113">适用于嵌入使用 HTTP GET （iframe 等） 的 URL</span><span class="sxs-lookup"><span data-stu-id="fd212-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="fd212-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="fd212-114">postUrl</span></span>        | <span data-ttu-id="fd212-115">string</span><span class="sxs-lookup"><span data-stu-id="fd212-115">string</span></span> | <span data-ttu-id="fd212-116">适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）</span><span class="sxs-lookup"><span data-stu-id="fd212-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="fd212-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="fd212-117">postParameters</span></span> | <span data-ttu-id="fd212-118">string</span><span class="sxs-lookup"><span data-stu-id="fd212-118">string</span></span> | <span data-ttu-id="fd212-119">如果使用 postUrl 包括 POST 参数</span><span class="sxs-lookup"><span data-stu-id="fd212-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="fd212-120">GetUrl、 postUrl，或同时可能会返回根据支持指定的选项的当前状态。</span><span class="sxs-lookup"><span data-stu-id="fd212-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="fd212-121">postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。</span><span class="sxs-lookup"><span data-stu-id="fd212-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="fd212-122">例如：</span><span class="sxs-lookup"><span data-stu-id="fd212-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="fd212-123">不透明应考虑的 Url 和参数的格式。</span><span class="sxs-lookup"><span data-stu-id="fd212-123">The formats of URLs and parameters should be considered opaque.</span></span>
