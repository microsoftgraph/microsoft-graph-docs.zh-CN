---
title: mediaInfo 资源类型
description: 操作中使用的媒体信息提示。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 65cf71f5c116fe213d0e32d560ec24704bff1172
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523979"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="43d3b-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="43d3b-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43d3b-104">操作中使用的媒体信息提示。</span><span class="sxs-lookup"><span data-stu-id="43d3b-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="43d3b-105">属性</span><span class="sxs-lookup"><span data-stu-id="43d3b-105">Properties</span></span>
| <span data-ttu-id="43d3b-106">属性</span><span class="sxs-lookup"><span data-stu-id="43d3b-106">Property</span></span>       | <span data-ttu-id="43d3b-107">类型</span><span class="sxs-lookup"><span data-stu-id="43d3b-107">Type</span></span>    | <span data-ttu-id="43d3b-108">说明</span><span class="sxs-lookup"><span data-stu-id="43d3b-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="43d3b-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="43d3b-109">resourceId</span></span>     | <span data-ttu-id="43d3b-110">String</span><span class="sxs-lookup"><span data-stu-id="43d3b-110">String</span></span>  | <span data-ttu-id="43d3b-111">唯一标识的资源。</span><span class="sxs-lookup"><span data-stu-id="43d3b-111">Unique identity of the resource.</span></span> |
| <span data-ttu-id="43d3b-112">uri</span><span class="sxs-lookup"><span data-stu-id="43d3b-112">uri</span></span>            | <span data-ttu-id="43d3b-113">String</span><span class="sxs-lookup"><span data-stu-id="43d3b-113">String</span></span>  | <span data-ttu-id="43d3b-114">资源的路径。</span><span class="sxs-lookup"><span data-stu-id="43d3b-114">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="43d3b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43d3b-115">JSON representation</span></span>

<span data-ttu-id="43d3b-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43d3b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediainfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
