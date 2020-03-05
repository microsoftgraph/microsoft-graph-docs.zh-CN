---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: ItemPreviewInfo 资源包含有关如何嵌入 driveItem 的预览的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7d2050a38e77e0cfa7176ba63756e9b9d8dcd384
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447623"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="043ad-103">itemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="043ad-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="043ad-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="043ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="043ad-105">**ItemPreviewInfo**资源包含有关如何嵌入[driveItem](driveitem.md)的预览的信息。</span><span class="sxs-lookup"><span data-stu-id="043ad-105">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="043ad-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="043ad-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="043ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="043ad-107">Properties</span></span>

| <span data-ttu-id="043ad-108">名称</span><span class="sxs-lookup"><span data-stu-id="043ad-108">Name</span></span>           | <span data-ttu-id="043ad-109">类型</span><span class="sxs-lookup"><span data-stu-id="043ad-109">Type</span></span>   | <span data-ttu-id="043ad-110">说明</span><span class="sxs-lookup"><span data-stu-id="043ad-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="043ad-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="043ad-111">getUrl</span></span>         | <span data-ttu-id="043ad-112">string</span><span class="sxs-lookup"><span data-stu-id="043ad-112">string</span></span> | <span data-ttu-id="043ad-113">适合使用 HTTP GET （iframe 等）进行嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="043ad-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="043ad-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="043ad-114">postUrl</span></span>        | <span data-ttu-id="043ad-115">string</span><span class="sxs-lookup"><span data-stu-id="043ad-115">string</span></span> | <span data-ttu-id="043ad-116">适合使用 HTTP POST （窗体 POST、JS 等）嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="043ad-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="043ad-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="043ad-117">postParameters</span></span> | <span data-ttu-id="043ad-118">string</span><span class="sxs-lookup"><span data-stu-id="043ad-118">string</span></span> | <span data-ttu-id="043ad-119">如果使用 postUrl，则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="043ad-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="043ad-120">根据指定选项的当前支持状态，可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="043ad-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="043ad-121">postParameters 是格式为`application/x-www-form-urlencoded`的字符串，如果向 POSTURL 执行 POST，应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="043ad-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="043ad-122">例如：</span><span class="sxs-lookup"><span data-stu-id="043ad-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="043ad-123">Url 和参数的格式应被认为是不透明的。</span><span class="sxs-lookup"><span data-stu-id="043ad-123">The formats of URLs and parameters should be considered opaque.</span></span>
