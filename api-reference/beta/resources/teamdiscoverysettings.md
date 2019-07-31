---
title: teamDiscoverySettings 资源类型
description: 用于配置他人的团队可发现性的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6dd1c3728d91be88689f72e020b773f7875807a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964569"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="e9fc5-103">teamDiscoverySettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9fc5-103">teamDiscoverySettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9fc5-104">提供允许其他人配置[团队](team.md)可发现性的设置。</span><span class="sxs-lookup"><span data-stu-id="e9fc5-104">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="e9fc5-105">您只能修改专用团队的发现设置。</span><span class="sxs-lookup"><span data-stu-id="e9fc5-105">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="e9fc5-106">属性</span><span class="sxs-lookup"><span data-stu-id="e9fc5-106">Properties</span></span>
| <span data-ttu-id="e9fc5-107">属性</span><span class="sxs-lookup"><span data-stu-id="e9fc5-107">Property</span></span>     | <span data-ttu-id="e9fc5-108">类型</span><span class="sxs-lookup"><span data-stu-id="e9fc5-108">Type</span></span>   |<span data-ttu-id="e9fc5-109">说明</span><span class="sxs-lookup"><span data-stu-id="e9fc5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9fc5-110">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="e9fc5-110">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="e9fc5-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9fc5-111">Boolean</span></span>|<span data-ttu-id="e9fc5-112">如果设置为 true, 则可以通过搜索和团队客户端的建议查看团队。</span><span class="sxs-lookup"><span data-stu-id="e9fc5-112">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9fc5-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9fc5-113">JSON representation</span></span>

<span data-ttu-id="e9fc5-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9fc5-114">The following is a JSON representation of the resource.</span></span>

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
