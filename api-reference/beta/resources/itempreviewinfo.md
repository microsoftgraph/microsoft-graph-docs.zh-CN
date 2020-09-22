---
author: kevinlam
description: ItemPreviewInfo 资源包含有关如何嵌入 DriveItem 的预览的信息。
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab62e2a41d257adcb8f763b77e42f0d7e515ee5b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033692"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="db716-103">ItemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="db716-103">ItemPreviewInfo resource type</span></span>

<span data-ttu-id="db716-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db716-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db716-105">**ItemPreviewInfo**资源包含有关如何嵌入[DriveItem](driveitem.md)的预览的信息。</span><span class="sxs-lookup"><span data-stu-id="db716-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="db716-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db716-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="db716-107">属性</span><span class="sxs-lookup"><span data-stu-id="db716-107">Properties</span></span>

| <span data-ttu-id="db716-108">名称</span><span class="sxs-lookup"><span data-stu-id="db716-108">Name</span></span>           | <span data-ttu-id="db716-109">类型</span><span class="sxs-lookup"><span data-stu-id="db716-109">Type</span></span>   | <span data-ttu-id="db716-110">说明</span><span class="sxs-lookup"><span data-stu-id="db716-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="db716-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="db716-111">getUrl</span></span>         | <span data-ttu-id="db716-112">string</span><span class="sxs-lookup"><span data-stu-id="db716-112">string</span></span> | <span data-ttu-id="db716-113">适用于使用 HTTP GET (iframe 等嵌入的 URL ) </span><span class="sxs-lookup"><span data-stu-id="db716-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="db716-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="db716-114">postUrl</span></span>        | <span data-ttu-id="db716-115">string</span><span class="sxs-lookup"><span data-stu-id="db716-115">string</span></span> | <span data-ttu-id="db716-116">适合使用 HTTP POST (表单 post、JS 等进行嵌入的 URL ) </span><span class="sxs-lookup"><span data-stu-id="db716-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="db716-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="db716-117">postParameters</span></span> | <span data-ttu-id="db716-118">string</span><span class="sxs-lookup"><span data-stu-id="db716-118">string</span></span> | <span data-ttu-id="db716-119">如果使用 postUrl，则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="db716-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="db716-120">根据指定选项的当前支持状态，可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="db716-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="db716-121">postParameters 是格式为的字符串 `application/x-www-form-urlencoded` ，如果向 postUrl 执行 POST，应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="db716-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="db716-122">例如：</span><span class="sxs-lookup"><span data-stu-id="db716-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="db716-123">Url 和参数的格式应被认为是不透明的。</span><span class="sxs-lookup"><span data-stu-id="db716-123">The formats of URLs and parameters should be considered opaque.</span></span>


