---
title: meetingInfo 资源类型
description: 会议指定要创建或加入会议的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c1126a3408b8353e927b5653fe60dd4a89125051
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509355"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="48662-103">meetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="48662-103">meetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48662-104">会议指定要创建或加入会议的信息。</span><span class="sxs-lookup"><span data-stu-id="48662-104">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="48662-105">属性</span><span class="sxs-lookup"><span data-stu-id="48662-105">Properties</span></span>

| <span data-ttu-id="48662-106">属性</span><span class="sxs-lookup"><span data-stu-id="48662-106">Property</span></span>       | <span data-ttu-id="48662-107">类型</span><span class="sxs-lookup"><span data-stu-id="48662-107">Type</span></span>    | <span data-ttu-id="48662-108">说明</span><span class="sxs-lookup"><span data-stu-id="48662-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48662-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="48662-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="48662-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="48662-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="48662-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48662-111">JSON representation</span></span>

<span data-ttu-id="48662-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48662-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
