---
title: teamFunSettings 资源类型
description: 要配置的团队中的使用 Giphy、 memes 和标签的设置。
localization_priority: Normal
ms.openlocfilehash: c53d3215e5f515361c66fe2d3d0ad10a5338e0c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852064"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="97596-103">teamFunSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="97596-103">teamFunSettings resource type</span></span>

> <span data-ttu-id="97596-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="97596-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97596-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97596-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97596-106">要配置的设置使用 Giphy、 memes 和[团队](team.md)中的标签。</span><span class="sxs-lookup"><span data-stu-id="97596-106">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="97596-107">属性</span><span class="sxs-lookup"><span data-stu-id="97596-107">Properties</span></span>
| <span data-ttu-id="97596-108">属性</span><span class="sxs-lookup"><span data-stu-id="97596-108">Property</span></span>     | <span data-ttu-id="97596-109">类型</span><span class="sxs-lookup"><span data-stu-id="97596-109">Type</span></span>   |<span data-ttu-id="97596-110">Description</span><span class="sxs-lookup"><span data-stu-id="97596-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97596-111">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="97596-111">allowGiphy</span></span>|<span data-ttu-id="97596-112">布尔</span><span class="sxs-lookup"><span data-stu-id="97596-112">Boolean</span></span>|<span data-ttu-id="97596-113">如果设置为 true，则启用 Giphy 使用。</span><span class="sxs-lookup"><span data-stu-id="97596-113">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="97596-114">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="97596-114">giphyContentRating</span></span>|<span data-ttu-id="97596-115">字符串 (enum)</span><span class="sxs-lookup"><span data-stu-id="97596-115">String (enum)</span></span>|<span data-ttu-id="97596-116">Giphy 内容评级。</span><span class="sxs-lookup"><span data-stu-id="97596-116">Giphy content rating.</span></span> <span data-ttu-id="97596-117">可取值为：`moderate`、`strict`。</span><span class="sxs-lookup"><span data-stu-id="97596-117">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="97596-118">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="97596-118">allowStickersAndMemes</span></span>|<span data-ttu-id="97596-119">布尔</span><span class="sxs-lookup"><span data-stu-id="97596-119">Boolean</span></span>|<span data-ttu-id="97596-120">如果设置为 true，使用户能够包括标签和 memes。</span><span class="sxs-lookup"><span data-stu-id="97596-120">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="97596-121">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="97596-121">allowCustomMemes</span></span>|<span data-ttu-id="97596-122">布尔</span><span class="sxs-lookup"><span data-stu-id="97596-122">Boolean</span></span>|<span data-ttu-id="97596-123">如果设置为 true，使用户能够包括自定义 memes。</span><span class="sxs-lookup"><span data-stu-id="97596-123">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97596-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97596-124">JSON representation</span></span>

<span data-ttu-id="97596-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97596-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
