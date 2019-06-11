---
title: teamDiscoverySettings 资源类型
description: 用于配置他人的团队可发现性的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 56284b678dec74e00724eeb429958aa54444208d
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2019
ms.locfileid: "34818699"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="f2441-103">teamDiscoverySettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2441-103">teamDiscoverySettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2441-104">提供允许其他人配置[团队](team.md)可发现性的设置。</span><span class="sxs-lookup"><span data-stu-id="f2441-104">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="f2441-105">您只能修改专用团队的发现设置。</span><span class="sxs-lookup"><span data-stu-id="f2441-105">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="f2441-106">属性</span><span class="sxs-lookup"><span data-stu-id="f2441-106">Properties</span></span>
| <span data-ttu-id="f2441-107">属性</span><span class="sxs-lookup"><span data-stu-id="f2441-107">Property</span></span>     | <span data-ttu-id="f2441-108">类型</span><span class="sxs-lookup"><span data-stu-id="f2441-108">Type</span></span>   |<span data-ttu-id="f2441-109">说明</span><span class="sxs-lookup"><span data-stu-id="f2441-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2441-110">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="f2441-110">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="f2441-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2441-111">Boolean</span></span>|<span data-ttu-id="f2441-112">如果设置为 true, 则可以通过搜索和团队客户端的建议查看团队。</span><span class="sxs-lookup"><span data-stu-id="f2441-112">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2441-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2441-113">JSON representation</span></span>

<span data-ttu-id="f2441-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2441-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamDiscoverySettings"
}-->

```json
{
  "showInTeamsSearchAndSuggestions": true
}
```

<!-- uuid: f1d42106-0b3d-4930-9f19-d76f4e03b36b
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's discoverySettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamdiscoverysettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
