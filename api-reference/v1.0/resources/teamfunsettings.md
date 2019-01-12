---
title: teamFunSettings 资源类型
description: 要配置的团队中的使用 Giphy、 memes 和标签的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987669"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="0a384-103">teamFunSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a384-103">teamFunSettings resource type</span></span>



<span data-ttu-id="0a384-104">要配置的设置使用 Giphy、 memes 和[团队](team.md)中的标签。</span><span class="sxs-lookup"><span data-stu-id="0a384-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0a384-105">属性</span><span class="sxs-lookup"><span data-stu-id="0a384-105">Properties</span></span>
| <span data-ttu-id="0a384-106">属性</span><span class="sxs-lookup"><span data-stu-id="0a384-106">Property</span></span>     | <span data-ttu-id="0a384-107">类型</span><span class="sxs-lookup"><span data-stu-id="0a384-107">Type</span></span>   |<span data-ttu-id="0a384-108">说明</span><span class="sxs-lookup"><span data-stu-id="0a384-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a384-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="0a384-109">allowGiphy</span></span>|<span data-ttu-id="0a384-110">布尔</span><span class="sxs-lookup"><span data-stu-id="0a384-110">Boolean</span></span>|<span data-ttu-id="0a384-111">如果设置为 true，则启用 Giphy 使用。</span><span class="sxs-lookup"><span data-stu-id="0a384-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="0a384-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="0a384-112">giphyContentRating</span></span>|<span data-ttu-id="0a384-113">字符串 (enum)</span><span class="sxs-lookup"><span data-stu-id="0a384-113">String (enum)</span></span>|<span data-ttu-id="0a384-114">Giphy 内容评级。</span><span class="sxs-lookup"><span data-stu-id="0a384-114">Giphy content rating.</span></span> <span data-ttu-id="0a384-115">可取值为：`moderate`、`strict`。</span><span class="sxs-lookup"><span data-stu-id="0a384-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="0a384-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="0a384-116">allowStickersAndMemes</span></span>|<span data-ttu-id="0a384-117">布尔</span><span class="sxs-lookup"><span data-stu-id="0a384-117">Boolean</span></span>|<span data-ttu-id="0a384-118">如果设置为 true，使用户能够包括标签和 memes。</span><span class="sxs-lookup"><span data-stu-id="0a384-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="0a384-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="0a384-119">allowCustomMemes</span></span>|<span data-ttu-id="0a384-120">布尔</span><span class="sxs-lookup"><span data-stu-id="0a384-120">Boolean</span></span>|<span data-ttu-id="0a384-121">如果设置为 true，使用户能够包括自定义 memes。</span><span class="sxs-lookup"><span data-stu-id="0a384-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a384-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a384-122">JSON representation</span></span>

<span data-ttu-id="0a384-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a384-123">The following is a JSON representation of the resource.</span></span>

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
