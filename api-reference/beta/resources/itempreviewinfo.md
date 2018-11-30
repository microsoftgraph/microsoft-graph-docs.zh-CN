---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
ms.openlocfilehash: 3fa9d10ae3aade7be96e81168b34df84698da1c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043134"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="dadcb-102">ItemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="dadcb-102">ItemPreviewInfo resource type</span></span>

> <span data-ttu-id="dadcb-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dadcb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dadcb-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dadcb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dadcb-105">**ItemPreviewInfo**资源包含有关如何将嵌入的[DriveItem](driveitem.md)预览信息。</span><span class="sxs-lookup"><span data-stu-id="dadcb-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="dadcb-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dadcb-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="dadcb-107">属性</span><span class="sxs-lookup"><span data-stu-id="dadcb-107">Properties</span></span>

| <span data-ttu-id="dadcb-108">名称</span><span class="sxs-lookup"><span data-stu-id="dadcb-108">Name</span></span>           | <span data-ttu-id="dadcb-109">类型</span><span class="sxs-lookup"><span data-stu-id="dadcb-109">Type</span></span>   | <span data-ttu-id="dadcb-110">说明</span><span class="sxs-lookup"><span data-stu-id="dadcb-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="dadcb-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="dadcb-111">getUrl</span></span>         | <span data-ttu-id="dadcb-112">string</span><span class="sxs-lookup"><span data-stu-id="dadcb-112">string</span></span> | <span data-ttu-id="dadcb-113">适用于嵌入使用 HTTP GET （iframe 等） 的 URL</span><span class="sxs-lookup"><span data-stu-id="dadcb-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="dadcb-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="dadcb-114">postUrl</span></span>        | <span data-ttu-id="dadcb-115">string</span><span class="sxs-lookup"><span data-stu-id="dadcb-115">string</span></span> | <span data-ttu-id="dadcb-116">适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）</span><span class="sxs-lookup"><span data-stu-id="dadcb-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="dadcb-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="dadcb-117">postParameters</span></span> | <span data-ttu-id="dadcb-118">string</span><span class="sxs-lookup"><span data-stu-id="dadcb-118">string</span></span> | <span data-ttu-id="dadcb-119">如果使用 postUrl 包括 POST 参数</span><span class="sxs-lookup"><span data-stu-id="dadcb-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="dadcb-120">GetUrl、 postUrl，或同时可能会返回根据支持指定的选项的当前状态。</span><span class="sxs-lookup"><span data-stu-id="dadcb-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="dadcb-121">postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。</span><span class="sxs-lookup"><span data-stu-id="dadcb-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="dadcb-122">例如：</span><span class="sxs-lookup"><span data-stu-id="dadcb-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="dadcb-123">不透明应考虑的 Url 和参数的格式。</span><span class="sxs-lookup"><span data-stu-id="dadcb-123">The formats of URLs and parameters should be considered opaque.</span></span>