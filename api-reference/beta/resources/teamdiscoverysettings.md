---
title: teamDiscoverySettings 资源类型
description: 用于让他人配置团队可发现性的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f26c47b2e1863c3108bc23f7c388179bd8006156
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046660"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="103e1-103">teamDiscoverySettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="103e1-103">teamDiscoverySettings resource type</span></span>

<span data-ttu-id="103e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="103e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="103e1-105">提供允许其他人配置 [团队](team.md) 可发现性的设置。</span><span class="sxs-lookup"><span data-stu-id="103e1-105">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="103e1-106">您只能修改专用团队的发现设置。</span><span class="sxs-lookup"><span data-stu-id="103e1-106">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="103e1-107">属性</span><span class="sxs-lookup"><span data-stu-id="103e1-107">Properties</span></span>
| <span data-ttu-id="103e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="103e1-108">Property</span></span>     | <span data-ttu-id="103e1-109">类型</span><span class="sxs-lookup"><span data-stu-id="103e1-109">Type</span></span>   |<span data-ttu-id="103e1-110">说明</span><span class="sxs-lookup"><span data-stu-id="103e1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="103e1-111">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="103e1-111">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="103e1-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="103e1-112">Boolean</span></span>|<span data-ttu-id="103e1-113">如果设置为 true，则可以通过搜索和团队客户端的建议查看团队。</span><span class="sxs-lookup"><span data-stu-id="103e1-113">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="103e1-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="103e1-114">JSON representation</span></span>

<span data-ttu-id="103e1-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="103e1-115">The following is a JSON representation of the resource.</span></span>

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


