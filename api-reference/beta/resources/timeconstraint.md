---
title: timeConstraint 资源类型
description: 根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。
ms.openlocfilehash: 092133d34e12fe5c06bfd8a76e8a33afb33892f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042698"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="76615-103">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="76615-103">timeConstraint resource type</span></span>

> <span data-ttu-id="76615-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="76615-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76615-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76615-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76615-106">根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。</span><span class="sxs-lookup"><span data-stu-id="76615-106">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76615-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76615-107">JSON representation</span></span>

<span data-ttu-id="76615-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76615-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="76615-109">属性</span><span class="sxs-lookup"><span data-stu-id="76615-109">Properties</span></span>
| <span data-ttu-id="76615-110">属性</span><span class="sxs-lookup"><span data-stu-id="76615-110">Property</span></span>     | <span data-ttu-id="76615-111">类型</span><span class="sxs-lookup"><span data-stu-id="76615-111">Type</span></span>   |<span data-ttu-id="76615-112">说明</span><span class="sxs-lookup"><span data-stu-id="76615-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76615-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="76615-113">activityDomain</span></span>|<span data-ttu-id="76615-114">字符串</span><span class="sxs-lookup"><span data-stu-id="76615-114">String</span></span>|<span data-ttu-id="76615-p102">（可选）活动性质。可取值为：`work`、`personal`、`unrestricted` 或 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="76615-p102">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="76615-117">timeslots</span><span class="sxs-lookup"><span data-stu-id="76615-117">timeslots</span></span>|<span data-ttu-id="76615-118">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76615-118">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="76615-119">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="76615-119">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->