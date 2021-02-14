---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: itemPreviewInfo 资源包含有关如何嵌入 driveItem 预览的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7ece7ed529a714b2e1262c4e39444639caced1
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240568"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="a2ea6-103">itemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2ea6-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="a2ea6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ea6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2ea6-105">**itemPreviewInfo** 资源包含有关如何嵌入 [driveItem](driveitem.md)预览的信息。</span><span class="sxs-lookup"><span data-stu-id="a2ea6-105">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2ea6-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2ea6-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="a2ea6-107">属性</span><span class="sxs-lookup"><span data-stu-id="a2ea6-107">Properties</span></span>

| <span data-ttu-id="a2ea6-108">名称</span><span class="sxs-lookup"><span data-stu-id="a2ea6-108">Name</span></span>           | <span data-ttu-id="a2ea6-109">类型</span><span class="sxs-lookup"><span data-stu-id="a2ea6-109">Type</span></span>   | <span data-ttu-id="a2ea6-110">说明</span><span class="sxs-lookup"><span data-stu-id="a2ea6-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="a2ea6-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="a2ea6-111">getUrl</span></span>         | <span data-ttu-id="a2ea6-112">string</span><span class="sxs-lookup"><span data-stu-id="a2ea6-112">string</span></span> | <span data-ttu-id="a2ea6-113">适合使用 HTTP GET (iframe 等嵌入的 URL) </span><span class="sxs-lookup"><span data-stu-id="a2ea6-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="a2ea6-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="a2ea6-114">postUrl</span></span>        | <span data-ttu-id="a2ea6-115">string</span><span class="sxs-lookup"><span data-stu-id="a2ea6-115">string</span></span> | <span data-ttu-id="a2ea6-116">适合使用 HTTP POST 和表单 (JS 等嵌入的 URL) </span><span class="sxs-lookup"><span data-stu-id="a2ea6-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="a2ea6-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="a2ea6-117">postParameters</span></span> | <span data-ttu-id="a2ea6-118">string</span><span class="sxs-lookup"><span data-stu-id="a2ea6-118">string</span></span> | <span data-ttu-id="a2ea6-119">使用 postUrl 时要包含的 POST 参数</span><span class="sxs-lookup"><span data-stu-id="a2ea6-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="a2ea6-120">可能会返回 getUrl、postUrl 或两者，具体取决于指定选项的当前支持状态。</span><span class="sxs-lookup"><span data-stu-id="a2ea6-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="a2ea6-121">postParameters 是格式设置为的字符串，如果对 postUrl 执行 `application/x-www-form-urlencoded` POST，应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="a2ea6-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="a2ea6-122">例如：</span><span class="sxs-lookup"><span data-stu-id="a2ea6-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="a2ea6-123">URL 和参数的格式应视为不透明。</span><span class="sxs-lookup"><span data-stu-id="a2ea6-123">The formats of URLs and parameters should be considered opaque.</span></span>

