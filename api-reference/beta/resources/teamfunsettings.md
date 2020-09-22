---
title: teamFunSettings 资源类型
description: 用于配置团队中 Giphy、成员和贴纸使用情况的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a58879c73e86dac6326576739c6a959a7e1efa78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046649"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="7f705-103">teamFunSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f705-103">teamFunSettings resource type</span></span>

<span data-ttu-id="7f705-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f705-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f705-105">用于配置在 [团队](team.md)中使用 Giphy、meme 和不干胶标签的设置。</span><span class="sxs-lookup"><span data-stu-id="7f705-105">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7f705-106">属性</span><span class="sxs-lookup"><span data-stu-id="7f705-106">Properties</span></span>
| <span data-ttu-id="7f705-107">属性</span><span class="sxs-lookup"><span data-stu-id="7f705-107">Property</span></span>     | <span data-ttu-id="7f705-108">类型</span><span class="sxs-lookup"><span data-stu-id="7f705-108">Type</span></span>   |<span data-ttu-id="7f705-109">说明</span><span class="sxs-lookup"><span data-stu-id="7f705-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f705-110">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="7f705-110">allowGiphy</span></span>|<span data-ttu-id="7f705-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f705-111">Boolean</span></span>|<span data-ttu-id="7f705-112">如果设置为 true，将启用 Giphy。</span><span class="sxs-lookup"><span data-stu-id="7f705-112">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="7f705-113">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="7f705-113">giphyContentRating</span></span>|<span data-ttu-id="7f705-114"> (枚举的字符串) </span><span class="sxs-lookup"><span data-stu-id="7f705-114">String (enum)</span></span>|<span data-ttu-id="7f705-115">Giphy 内容评级。</span><span class="sxs-lookup"><span data-stu-id="7f705-115">Giphy content rating.</span></span> <span data-ttu-id="7f705-116">可取值为：`moderate`、`strict`。</span><span class="sxs-lookup"><span data-stu-id="7f705-116">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="7f705-117">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="7f705-117">allowStickersAndMemes</span></span>|<span data-ttu-id="7f705-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f705-118">Boolean</span></span>|<span data-ttu-id="7f705-119">如果设置为 true，则允许用户包括不干胶标签和 meme。</span><span class="sxs-lookup"><span data-stu-id="7f705-119">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="7f705-120">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="7f705-120">allowCustomMemes</span></span>|<span data-ttu-id="7f705-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f705-121">Boolean</span></span>|<span data-ttu-id="7f705-122">如果设置为 true，则允许用户包含自定义 meme。</span><span class="sxs-lookup"><span data-stu-id="7f705-122">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f705-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f705-123">JSON representation</span></span>

<span data-ttu-id="7f705-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f705-124">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


