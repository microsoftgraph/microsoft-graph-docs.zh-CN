---
title: commsNotifications 资源类型
description: Communications server 用于在单一批次中发送多个通知的通知的列表。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2d002b74bffe0911e2ba1fef4eed324b52ebcc49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520590"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="15173-103">commsNotifications 资源类型</span><span class="sxs-lookup"><span data-stu-id="15173-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15173-104">Communications server 用于在单一批次中发送多个通知的通知的列表。</span><span class="sxs-lookup"><span data-stu-id="15173-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="15173-105">属性</span><span class="sxs-lookup"><span data-stu-id="15173-105">Properties</span></span>

| <span data-ttu-id="15173-106">属性</span><span class="sxs-lookup"><span data-stu-id="15173-106">Property</span></span>       | <span data-ttu-id="15173-107">类型</span><span class="sxs-lookup"><span data-stu-id="15173-107">Type</span></span>                                                 | <span data-ttu-id="15173-108">说明</span><span class="sxs-lookup"><span data-stu-id="15173-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="15173-109">value</span><span class="sxs-lookup"><span data-stu-id="15173-109">value</span></span>          | <span data-ttu-id="15173-110">[commsNotification](commsnotification.md)集合</span><span class="sxs-lookup"><span data-stu-id="15173-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="15173-111">资源中更改的通知。</span><span class="sxs-lookup"><span data-stu-id="15173-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15173-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15173-112">JSON representation</span></span>

<span data-ttu-id="15173-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15173-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsnotifications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
