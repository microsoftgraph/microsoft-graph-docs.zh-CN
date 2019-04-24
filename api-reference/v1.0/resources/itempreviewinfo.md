---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
ms.openlocfilehash: e7df636f9c406a499baa5ef3be1748273920cac4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585235"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="5611b-102">itemPreviewInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5611b-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="5611b-103">**itemPreviewInfo**资源包含有关如何嵌入[driveItem](driveitem.md)的预览的信息。</span><span class="sxs-lookup"><span data-stu-id="5611b-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5611b-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5611b-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="5611b-105">属性</span><span class="sxs-lookup"><span data-stu-id="5611b-105">Properties</span></span>

| <span data-ttu-id="5611b-106">名称</span><span class="sxs-lookup"><span data-stu-id="5611b-106">Name</span></span>           | <span data-ttu-id="5611b-107">类型</span><span class="sxs-lookup"><span data-stu-id="5611b-107">Type</span></span>   | <span data-ttu-id="5611b-108">说明</span><span class="sxs-lookup"><span data-stu-id="5611b-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="5611b-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="5611b-109">getUrl</span></span>         | <span data-ttu-id="5611b-110">字符串</span><span class="sxs-lookup"><span data-stu-id="5611b-110">string</span></span> | <span data-ttu-id="5611b-111">适合使用 HTTP GET (iframe 等) 进行嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="5611b-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="5611b-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="5611b-112">postUrl</span></span>        | <span data-ttu-id="5611b-113">字符串</span><span class="sxs-lookup"><span data-stu-id="5611b-113">string</span></span> | <span data-ttu-id="5611b-114">适合使用 HTTP POST (窗体 POST、JS 等) 嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="5611b-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="5611b-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="5611b-115">postParameters</span></span> | <span data-ttu-id="5611b-116">字符串</span><span class="sxs-lookup"><span data-stu-id="5611b-116">string</span></span> | <span data-ttu-id="5611b-117">如果使用 postUrl, 则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="5611b-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="5611b-118">根据指定选项的当前支持状态, 可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="5611b-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="5611b-119">postParameters 是格式为`application/x-www-form-urlencoded`的字符串, 如果向 postUrl 执行 POST, 应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="5611b-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="5611b-120">例如：</span><span class="sxs-lookup"><span data-stu-id="5611b-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="5611b-121">url 和参数的格式应被认为是不透明的。</span><span class="sxs-lookup"><span data-stu-id="5611b-121">The formats of URLs and parameters should be considered opaque.</span></span>
