---
author: kevinlam
description: ItemPreviewInfo 资源包含有关如何嵌入 DriveItem 的预览的信息。
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4e4a26a9db6ebf4cbedb37fb60b177fa837c16d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523056"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="09e40-103">ItemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="09e40-103">ItemPreviewInfo resource type</span></span>

<span data-ttu-id="09e40-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="09e40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09e40-105">**ItemPreviewInfo**资源包含有关如何嵌入[DriveItem](driveitem.md)的预览的信息。</span><span class="sxs-lookup"><span data-stu-id="09e40-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="09e40-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09e40-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="09e40-107">属性</span><span class="sxs-lookup"><span data-stu-id="09e40-107">Properties</span></span>

| <span data-ttu-id="09e40-108">名称</span><span class="sxs-lookup"><span data-stu-id="09e40-108">Name</span></span>           | <span data-ttu-id="09e40-109">类型</span><span class="sxs-lookup"><span data-stu-id="09e40-109">Type</span></span>   | <span data-ttu-id="09e40-110">说明</span><span class="sxs-lookup"><span data-stu-id="09e40-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="09e40-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="09e40-111">getUrl</span></span>         | <span data-ttu-id="09e40-112">string</span><span class="sxs-lookup"><span data-stu-id="09e40-112">string</span></span> | <span data-ttu-id="09e40-113">适合使用 HTTP GET （iframe 等）进行嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="09e40-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="09e40-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="09e40-114">postUrl</span></span>        | <span data-ttu-id="09e40-115">string</span><span class="sxs-lookup"><span data-stu-id="09e40-115">string</span></span> | <span data-ttu-id="09e40-116">适合使用 HTTP POST （窗体 POST、JS 等）嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="09e40-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="09e40-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="09e40-117">postParameters</span></span> | <span data-ttu-id="09e40-118">string</span><span class="sxs-lookup"><span data-stu-id="09e40-118">string</span></span> | <span data-ttu-id="09e40-119">如果使用 postUrl，则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="09e40-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="09e40-120">根据指定选项的当前支持状态，可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="09e40-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="09e40-121">postParameters 是格式为`application/x-www-form-urlencoded`的字符串，如果向 POSTURL 执行 POST，应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="09e40-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="09e40-122">例如：</span><span class="sxs-lookup"><span data-stu-id="09e40-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="09e40-123">Url 和参数的格式应被认为是不透明的。</span><span class="sxs-lookup"><span data-stu-id="09e40-123">The formats of URLs and parameters should be considered opaque.</span></span>
