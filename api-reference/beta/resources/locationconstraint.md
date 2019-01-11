---
title: locationConstraint 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
ms.openlocfilehash: b1ff078efd5608fa388587003cf904c2b995f12e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851525"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="5b75d-103">locationConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b75d-103">locationConstraint resource type</span></span>

> <span data-ttu-id="5b75d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b75d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b75d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b75d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b75d-106">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="5b75d-106">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b75d-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b75d-107">JSON representation</span></span>

<span data-ttu-id="5b75d-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b75d-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationconstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="5b75d-109">属性</span><span class="sxs-lookup"><span data-stu-id="5b75d-109">Properties</span></span>
| <span data-ttu-id="5b75d-110">属性</span><span class="sxs-lookup"><span data-stu-id="5b75d-110">Property</span></span>     | <span data-ttu-id="5b75d-111">类型</span><span class="sxs-lookup"><span data-stu-id="5b75d-111">Type</span></span>   |<span data-ttu-id="5b75d-112">说明</span><span class="sxs-lookup"><span data-stu-id="5b75d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b75d-113">isRequired</span><span class="sxs-lookup"><span data-stu-id="5b75d-113">isRequired</span></span>|<span data-ttu-id="5b75d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b75d-114">Boolean</span></span>|<span data-ttu-id="5b75d-p102">客户端请求服务在响应中添加会议地点。若为 true，且所有资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 将不会返回任何会议时间建议。若为 false，且所有资源处于忙碌状态，**findMeetingTimes** 仍会在没有会议地点的情况下查找会议时间。</span><span class="sxs-lookup"><span data-stu-id="5b75d-p102">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="5b75d-118">locations</span><span class="sxs-lookup"><span data-stu-id="5b75d-118">locations</span></span>|<span data-ttu-id="5b75d-119">[locationConstraintItem](locationconstraintitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b75d-119">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="5b75d-120">客户端请求的一个或多个会议地点的约束信息。</span><span class="sxs-lookup"><span data-stu-id="5b75d-120">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="5b75d-121">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="5b75d-121">suggestLocation</span></span>|<span data-ttu-id="5b75d-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b75d-122">Boolean</span></span>|<span data-ttu-id="5b75d-123">客户端请求服务返回一个或多个会议地点建议。</span><span class="sxs-lookup"><span data-stu-id="5b75d-123">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
