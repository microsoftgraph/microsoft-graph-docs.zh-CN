---
title: teamFunSettings 资源类型
description: 用于配置团队中 Giphy、成员和贴纸使用情况的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548514"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="23b88-103">teamFunSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="23b88-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23b88-104">用于配置在[团队](team.md)中使用 Giphy、meme 和不干胶标签的设置。</span><span class="sxs-lookup"><span data-stu-id="23b88-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="23b88-105">属性</span><span class="sxs-lookup"><span data-stu-id="23b88-105">Properties</span></span>
| <span data-ttu-id="23b88-106">属性</span><span class="sxs-lookup"><span data-stu-id="23b88-106">Property</span></span>     | <span data-ttu-id="23b88-107">类型</span><span class="sxs-lookup"><span data-stu-id="23b88-107">Type</span></span>   |<span data-ttu-id="23b88-108">说明</span><span class="sxs-lookup"><span data-stu-id="23b88-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23b88-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="23b88-109">allowGiphy</span></span>|<span data-ttu-id="23b88-110">布尔值</span><span class="sxs-lookup"><span data-stu-id="23b88-110">Boolean</span></span>|<span data-ttu-id="23b88-111">如果设置为 true, 将启用 Giphy。</span><span class="sxs-lookup"><span data-stu-id="23b88-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="23b88-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="23b88-112">giphyContentRating</span></span>|<span data-ttu-id="23b88-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="23b88-113">String (enum)</span></span>|<span data-ttu-id="23b88-114">Giphy 内容评级。</span><span class="sxs-lookup"><span data-stu-id="23b88-114">Giphy content rating.</span></span> <span data-ttu-id="23b88-115">可取值为：`moderate`、`strict`。</span><span class="sxs-lookup"><span data-stu-id="23b88-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="23b88-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="23b88-116">allowStickersAndMemes</span></span>|<span data-ttu-id="23b88-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="23b88-117">Boolean</span></span>|<span data-ttu-id="23b88-118">如果设置为 true, 则允许用户包括不干胶标签和 meme。</span><span class="sxs-lookup"><span data-stu-id="23b88-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="23b88-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="23b88-119">allowCustomMemes</span></span>|<span data-ttu-id="23b88-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="23b88-120">Boolean</span></span>|<span data-ttu-id="23b88-121">如果设置为 true, 则允许用户包含自定义 meme。</span><span class="sxs-lookup"><span data-stu-id="23b88-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23b88-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23b88-122">JSON representation</span></span>

<span data-ttu-id="23b88-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23b88-123">The following is a JSON representation of the resource.</span></span>

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
