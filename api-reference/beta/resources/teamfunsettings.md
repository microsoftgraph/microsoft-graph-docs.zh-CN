---
title: teamFunSettings 资源类型
description: 用于配置团队中 Giphy、成员和贴纸使用情况的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: dc8d4cfa05f7bc6cbda9dfbf5d113370a1981ba5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515858"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="5e807-103">teamFunSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e807-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e807-104">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="5e807-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e807-105">属性</span><span class="sxs-lookup"><span data-stu-id="5e807-105">Properties</span></span>
| <span data-ttu-id="5e807-106">属性</span><span class="sxs-lookup"><span data-stu-id="5e807-106">Property</span></span>     | <span data-ttu-id="5e807-107">类型</span><span class="sxs-lookup"><span data-stu-id="5e807-107">Type</span></span>   |<span data-ttu-id="5e807-108">说明</span><span class="sxs-lookup"><span data-stu-id="5e807-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e807-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="5e807-109">allowGiphy</span></span>|<span data-ttu-id="5e807-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e807-110">Boolean</span></span>|<span data-ttu-id="5e807-111">如果设置为 true，则启用 Giphy 使用。</span><span class="sxs-lookup"><span data-stu-id="5e807-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="5e807-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="5e807-112">giphyContentRating</span></span>|<span data-ttu-id="5e807-113">字符串 (enum)</span><span class="sxs-lookup"><span data-stu-id="5e807-113">String (enum)</span></span>|<span data-ttu-id="5e807-114">Giphy 内容评级。</span><span class="sxs-lookup"><span data-stu-id="5e807-114">Giphy content rating.</span></span> <span data-ttu-id="5e807-115">可取值为：`moderate`、`strict`。</span><span class="sxs-lookup"><span data-stu-id="5e807-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="5e807-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="5e807-116">allowStickersAndMemes</span></span>|<span data-ttu-id="5e807-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e807-117">Boolean</span></span>|<span data-ttu-id="5e807-118">如果设置为 true，使用户能够包括标签和 memes。</span><span class="sxs-lookup"><span data-stu-id="5e807-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="5e807-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="5e807-119">allowCustomMemes</span></span>|<span data-ttu-id="5e807-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e807-120">Boolean</span></span>|<span data-ttu-id="5e807-121">如果设置为 true，使用户能够包括自定义 memes。</span><span class="sxs-lookup"><span data-stu-id="5e807-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e807-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e807-122">JSON representation</span></span>

<span data-ttu-id="5e807-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e807-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
