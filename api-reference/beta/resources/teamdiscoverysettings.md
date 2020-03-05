---
title: teamDiscoverySettings 资源类型
description: 用于让他人配置团队可发现性的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9a668c9d3b234fede0ad5c151e1dbbc95fc93516
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519958"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="287e0-103">teamDiscoverySettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="287e0-103">teamDiscoverySettings resource type</span></span>

<span data-ttu-id="287e0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="287e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="287e0-105">提供允许其他人配置[团队](team.md)可发现性的设置。</span><span class="sxs-lookup"><span data-stu-id="287e0-105">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="287e0-106">您只能修改专用团队的发现设置。</span><span class="sxs-lookup"><span data-stu-id="287e0-106">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="287e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="287e0-107">Properties</span></span>
| <span data-ttu-id="287e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="287e0-108">Property</span></span>     | <span data-ttu-id="287e0-109">类型</span><span class="sxs-lookup"><span data-stu-id="287e0-109">Type</span></span>   |<span data-ttu-id="287e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="287e0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="287e0-111">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="287e0-111">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="287e0-112">布尔</span><span class="sxs-lookup"><span data-stu-id="287e0-112">Boolean</span></span>|<span data-ttu-id="287e0-113">如果设置为 true，则可以通过搜索和团队客户端的建议查看团队。</span><span class="sxs-lookup"><span data-stu-id="287e0-113">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="287e0-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="287e0-114">JSON representation</span></span>

<span data-ttu-id="287e0-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="287e0-115">The following is a JSON representation of the resource.</span></span>

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
