---
title: locationConstraint 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6828d7afdb9caec79978f4196106ff687faa2a1d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009935"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="c0f88-103">locationConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0f88-103">locationConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f88-104">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="c0f88-104">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0f88-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0f88-105">JSON representation</span></span>

<span data-ttu-id="c0f88-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0f88-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="c0f88-107">属性</span><span class="sxs-lookup"><span data-stu-id="c0f88-107">Properties</span></span>
| <span data-ttu-id="c0f88-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0f88-108">Property</span></span>     | <span data-ttu-id="c0f88-109">类型</span><span class="sxs-lookup"><span data-stu-id="c0f88-109">Type</span></span>   |<span data-ttu-id="c0f88-110">说明</span><span class="sxs-lookup"><span data-stu-id="c0f88-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0f88-111">isRequired</span><span class="sxs-lookup"><span data-stu-id="c0f88-111">isRequired</span></span>|<span data-ttu-id="c0f88-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f88-112">Boolean</span></span>|<span data-ttu-id="c0f88-p101">客户端请求服务在响应中添加会议地点。若为 true，且所有资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 将不会返回任何会议时间建议。若为 false，且所有资源处于忙碌状态，**findMeetingTimes** 仍会在没有会议地点的情况下查找会议时间。</span><span class="sxs-lookup"><span data-stu-id="c0f88-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="c0f88-116">locations</span><span class="sxs-lookup"><span data-stu-id="c0f88-116">locations</span></span>|<span data-ttu-id="c0f88-117">[locationConstraintItem](locationconstraintitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0f88-117">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="c0f88-118">客户端请求的一个或多个会议地点的约束信息。</span><span class="sxs-lookup"><span data-stu-id="c0f88-118">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="c0f88-119">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="c0f88-119">suggestLocation</span></span>|<span data-ttu-id="c0f88-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f88-120">Boolean</span></span>|<span data-ttu-id="c0f88-121">客户端请求服务返回一个或多个会议地点建议。</span><span class="sxs-lookup"><span data-stu-id="c0f88-121">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
