---
title: locationConstraints 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b9ac80069a7ffe61171a9e24feb2e65895c469bd
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057344"
---
# <a name="locationconstraints-resource-type"></a><span data-ttu-id="748af-103">locationConstraints 资源类型</span><span class="sxs-lookup"><span data-stu-id="748af-103">locationConstraints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="748af-104">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="748af-104">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="748af-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="748af-105">JSON representation</span></span>

<span data-ttu-id="748af-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="748af-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraints"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="748af-107">属性</span><span class="sxs-lookup"><span data-stu-id="748af-107">Properties</span></span>
| <span data-ttu-id="748af-108">属性</span><span class="sxs-lookup"><span data-stu-id="748af-108">Property</span></span>     | <span data-ttu-id="748af-109">类型</span><span class="sxs-lookup"><span data-stu-id="748af-109">Type</span></span>   |<span data-ttu-id="748af-110">说明</span><span class="sxs-lookup"><span data-stu-id="748af-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="748af-111">isRequired</span><span class="sxs-lookup"><span data-stu-id="748af-111">isRequired</span></span>|<span data-ttu-id="748af-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="748af-112">Boolean</span></span>|<span data-ttu-id="748af-p101">客户端请求服务在响应中添加会议地点。若为 true，且所有资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 将不会返回任何会议时间建议。若为 false，且所有资源处于忙碌状态，**findMeetingTimes** 仍会在没有会议地点的情况下查找会议时间。</span><span class="sxs-lookup"><span data-stu-id="748af-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="748af-116">位置</span><span class="sxs-lookup"><span data-stu-id="748af-116">locations</span></span>|<span data-ttu-id="748af-117">[locationConstraintItem](locationconstraintitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="748af-117">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="748af-118">客户端请求的一个或多个会议地点的约束信息。</span><span class="sxs-lookup"><span data-stu-id="748af-118">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="748af-119">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="748af-119">suggestLocation</span></span>|<span data-ttu-id="748af-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="748af-120">Boolean</span></span>|<span data-ttu-id="748af-121">客户端请求服务返回一个或多个会议地点建议。</span><span class="sxs-lookup"><span data-stu-id="748af-121">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->