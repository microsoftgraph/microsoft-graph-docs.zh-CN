---
title: teamDiscoverySettings 资源类型
description: 用于让他人配置团队可发现性的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: edc3c6cc446e35f2f5a97212d3c0b6f69b81ce30
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292883"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="731b5-103">teamDiscoverySettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="731b5-103">teamDiscoverySettings resource type</span></span>

<span data-ttu-id="731b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="731b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="731b5-105">提供允许其他人配置团队可发现 [性的](team.md) 设置。</span><span class="sxs-lookup"><span data-stu-id="731b5-105">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="731b5-106">只能修改私人团队的发现设置。</span><span class="sxs-lookup"><span data-stu-id="731b5-106">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="731b5-107">属性</span><span class="sxs-lookup"><span data-stu-id="731b5-107">Properties</span></span>
| <span data-ttu-id="731b5-108">属性</span><span class="sxs-lookup"><span data-stu-id="731b5-108">Property</span></span>     | <span data-ttu-id="731b5-109">类型</span><span class="sxs-lookup"><span data-stu-id="731b5-109">Type</span></span>   |<span data-ttu-id="731b5-110">说明</span><span class="sxs-lookup"><span data-stu-id="731b5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="731b5-111">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="731b5-111">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="731b5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="731b5-112">Boolean</span></span>|<span data-ttu-id="731b5-113">如果设置为 true，则团队可通过 Teams 客户端中的搜索和建议显示。</span><span class="sxs-lookup"><span data-stu-id="731b5-113">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="731b5-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="731b5-114">JSON representation</span></span>

<span data-ttu-id="731b5-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="731b5-115">The following is a JSON representation of the resource.</span></span>

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
  ]
}-->


