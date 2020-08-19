---
title: locationConstraint 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c2646e361e81b5d9ec0c45e3bcfe5f867c5ebe97
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807764"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="aae67-103">locationConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="aae67-103">locationConstraint resource type</span></span>

<span data-ttu-id="aae67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aae67-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aae67-105">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="aae67-105">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aae67-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aae67-106">JSON representation</span></span>

<span data-ttu-id="aae67-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aae67-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="aae67-108">属性</span><span class="sxs-lookup"><span data-stu-id="aae67-108">Properties</span></span>
| <span data-ttu-id="aae67-109">属性</span><span class="sxs-lookup"><span data-stu-id="aae67-109">Property</span></span>     | <span data-ttu-id="aae67-110">类型</span><span class="sxs-lookup"><span data-stu-id="aae67-110">Type</span></span>   |<span data-ttu-id="aae67-111">说明</span><span class="sxs-lookup"><span data-stu-id="aae67-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aae67-112">isRequired</span><span class="sxs-lookup"><span data-stu-id="aae67-112">isRequired</span></span>|<span data-ttu-id="aae67-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="aae67-113">Boolean</span></span>|<span data-ttu-id="aae67-p101">客户端请求服务在响应中添加会议地点。若为 true，且所有资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 将不会返回任何会议时间建议。若为 false，且所有资源处于忙碌状态，**findMeetingTimes** 仍会在没有会议地点的情况下查找会议时间。</span><span class="sxs-lookup"><span data-stu-id="aae67-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="aae67-117">locations</span><span class="sxs-lookup"><span data-stu-id="aae67-117">locations</span></span>|<span data-ttu-id="aae67-118">[locationConstraintItem](locationconstraintitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aae67-118">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="aae67-119">客户端请求的一个或多个会议地点的约束信息。</span><span class="sxs-lookup"><span data-stu-id="aae67-119">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="aae67-120">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="aae67-120">suggestLocation</span></span>|<span data-ttu-id="aae67-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="aae67-121">Boolean</span></span>|<span data-ttu-id="aae67-122">客户端请求服务返回一个或多个会议地点建议。</span><span class="sxs-lookup"><span data-stu-id="aae67-122">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
