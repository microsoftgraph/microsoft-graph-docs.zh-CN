---
title: teamFunSettings 资源类型
description: 用于配置团队中 Giphy、成员和贴纸使用情况的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 696a6a3b02f90abe1456f99d9a40a4d9127b5697
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533548"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="1456e-103">teamFunSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="1456e-103">teamFunSettings resource type</span></span>

<span data-ttu-id="1456e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1456e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="1456e-105">用于配置在[团队](team.md)中使用 Giphy、meme 和不干胶标签的设置。</span><span class="sxs-lookup"><span data-stu-id="1456e-105">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1456e-106">属性</span><span class="sxs-lookup"><span data-stu-id="1456e-106">Properties</span></span>
| <span data-ttu-id="1456e-107">属性</span><span class="sxs-lookup"><span data-stu-id="1456e-107">Property</span></span>     | <span data-ttu-id="1456e-108">类型</span><span class="sxs-lookup"><span data-stu-id="1456e-108">Type</span></span>   |<span data-ttu-id="1456e-109">说明</span><span class="sxs-lookup"><span data-stu-id="1456e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1456e-110">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="1456e-110">allowGiphy</span></span>|<span data-ttu-id="1456e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1456e-111">Boolean</span></span>|<span data-ttu-id="1456e-112">如果设置为 true，将启用 Giphy。</span><span class="sxs-lookup"><span data-stu-id="1456e-112">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="1456e-113">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="1456e-113">giphyContentRating</span></span>|<span data-ttu-id="1456e-114">String （enum）</span><span class="sxs-lookup"><span data-stu-id="1456e-114">String (enum)</span></span>|<span data-ttu-id="1456e-115">Giphy 内容评级。</span><span class="sxs-lookup"><span data-stu-id="1456e-115">Giphy content rating.</span></span> <span data-ttu-id="1456e-116">可取值为：`moderate`、`strict`。</span><span class="sxs-lookup"><span data-stu-id="1456e-116">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="1456e-117">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="1456e-117">allowStickersAndMemes</span></span>|<span data-ttu-id="1456e-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="1456e-118">Boolean</span></span>|<span data-ttu-id="1456e-119">如果设置为 true，则允许用户包括不干胶标签和 meme。</span><span class="sxs-lookup"><span data-stu-id="1456e-119">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="1456e-120">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="1456e-120">allowCustomMemes</span></span>|<span data-ttu-id="1456e-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="1456e-121">Boolean</span></span>|<span data-ttu-id="1456e-122">如果设置为 true，则允许用户包含自定义 meme。</span><span class="sxs-lookup"><span data-stu-id="1456e-122">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1456e-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1456e-123">JSON representation</span></span>

<span data-ttu-id="1456e-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1456e-124">The following is a JSON representation of the resource.</span></span>

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
