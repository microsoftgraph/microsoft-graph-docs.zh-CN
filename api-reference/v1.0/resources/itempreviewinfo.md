---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: ItemPreviewInfo 资源包含有关如何嵌入 driveItem 的预览的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71d660a71bce09f198a0feb9c3acbb9a69a23a5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036559"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="45ef4-103">itemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="45ef4-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="45ef4-104">**ItemPreviewInfo**资源包含有关如何嵌入[driveItem](driveitem.md)的预览的信息。</span><span class="sxs-lookup"><span data-stu-id="45ef4-104">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="45ef4-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45ef4-105">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="45ef4-106">属性</span><span class="sxs-lookup"><span data-stu-id="45ef4-106">Properties</span></span>

| <span data-ttu-id="45ef4-107">名称</span><span class="sxs-lookup"><span data-stu-id="45ef4-107">Name</span></span>           | <span data-ttu-id="45ef4-108">类型</span><span class="sxs-lookup"><span data-stu-id="45ef4-108">Type</span></span>   | <span data-ttu-id="45ef4-109">说明</span><span class="sxs-lookup"><span data-stu-id="45ef4-109">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="45ef4-110">getUrl</span><span class="sxs-lookup"><span data-stu-id="45ef4-110">getUrl</span></span>         | <span data-ttu-id="45ef4-111">string</span><span class="sxs-lookup"><span data-stu-id="45ef4-111">string</span></span> | <span data-ttu-id="45ef4-112">适合使用 HTTP GET (iframe 等) 进行嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="45ef4-112">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="45ef4-113">postUrl</span><span class="sxs-lookup"><span data-stu-id="45ef4-113">postUrl</span></span>        | <span data-ttu-id="45ef4-114">string</span><span class="sxs-lookup"><span data-stu-id="45ef4-114">string</span></span> | <span data-ttu-id="45ef4-115">适合使用 HTTP POST (窗体 POST、JS 等) 嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="45ef4-115">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="45ef4-116">postParameters</span><span class="sxs-lookup"><span data-stu-id="45ef4-116">postParameters</span></span> | <span data-ttu-id="45ef4-117">string</span><span class="sxs-lookup"><span data-stu-id="45ef4-117">string</span></span> | <span data-ttu-id="45ef4-118">如果使用 postUrl, 则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="45ef4-118">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="45ef4-119">根据指定选项的当前支持状态, 可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="45ef4-119">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="45ef4-120">postParameters 是格式为`application/x-www-form-urlencoded`的字符串, 如果向 POSTURL 执行 POST, 应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="45ef4-120">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="45ef4-121">例如：</span><span class="sxs-lookup"><span data-stu-id="45ef4-121">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="45ef4-122">Url 和参数的格式应被认为是不透明的。</span><span class="sxs-lookup"><span data-stu-id="45ef4-122">The formats of URLs and parameters should be considered opaque.</span></span>
