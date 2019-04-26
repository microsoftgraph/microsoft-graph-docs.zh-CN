---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 65cf71f5c116fe213d0e32d560ec24704bff1172
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562601"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="2edf0-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="2edf0-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2edf0-104">在提示操作中使用的媒体信息。</span><span class="sxs-lookup"><span data-stu-id="2edf0-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="2edf0-105">属性</span><span class="sxs-lookup"><span data-stu-id="2edf0-105">Properties</span></span>
| <span data-ttu-id="2edf0-106">属性</span><span class="sxs-lookup"><span data-stu-id="2edf0-106">Property</span></span>       | <span data-ttu-id="2edf0-107">类型</span><span class="sxs-lookup"><span data-stu-id="2edf0-107">Type</span></span>    | <span data-ttu-id="2edf0-108">说明</span><span class="sxs-lookup"><span data-stu-id="2edf0-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="2edf0-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="2edf0-109">resourceId</span></span>     | <span data-ttu-id="2edf0-110">String</span><span class="sxs-lookup"><span data-stu-id="2edf0-110">String</span></span>  | <span data-ttu-id="2edf0-111">资源的唯一标识。</span><span class="sxs-lookup"><span data-stu-id="2edf0-111">Unique identity of the resource.</span></span> |
| <span data-ttu-id="2edf0-112">url</span><span class="sxs-lookup"><span data-stu-id="2edf0-112">uri</span></span>            | <span data-ttu-id="2edf0-113">String</span><span class="sxs-lookup"><span data-stu-id="2edf0-113">String</span></span>  | <span data-ttu-id="2edf0-114">资源的路径。</span><span class="sxs-lookup"><span data-stu-id="2edf0-114">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="2edf0-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2edf0-115">JSON representation</span></span>

<span data-ttu-id="2edf0-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2edf0-116">The following is a JSON representation of the resource.</span></span>

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
