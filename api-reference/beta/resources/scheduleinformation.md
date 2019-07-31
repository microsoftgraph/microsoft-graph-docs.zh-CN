---
title: scheduleInformation 资源类型
description: '表示用户、通讯组列表或资源在指定时间段内的可用性。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: 3d6ede4e1085a8be3f78b714f690b79b836abbcb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965304"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="65596-103">scheduleInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="65596-103">scheduleInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="65596-104">表示用户、通讯组列表或资源 (会议室或设备) 在指定时间段的可用性。</span><span class="sxs-lookup"><span data-stu-id="65596-104">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="65596-105">属性</span><span class="sxs-lookup"><span data-stu-id="65596-105">Properties</span></span>
| <span data-ttu-id="65596-106">属性</span><span class="sxs-lookup"><span data-stu-id="65596-106">Property</span></span>     | <span data-ttu-id="65596-107">类型</span><span class="sxs-lookup"><span data-stu-id="65596-107">Type</span></span>   |<span data-ttu-id="65596-108">说明</span><span class="sxs-lookup"><span data-stu-id="65596-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65596-109">availabilityView</span><span class="sxs-lookup"><span data-stu-id="65596-109">availabilityView</span></span> |<span data-ttu-id="65596-110">String</span><span class="sxs-lookup"><span data-stu-id="65596-110">String</span></span> |<span data-ttu-id="65596-111">表示中`scheduleItems`所有项的可用性的合并视图。</span><span class="sxs-lookup"><span data-stu-id="65596-111">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="65596-112">视图由时间段组成。</span><span class="sxs-lookup"><span data-stu-id="65596-112">The view consists of time slots.</span></span> <span data-ttu-id="65596-113">在每个时间段内的可用性表示`0`为: = `1`free、= `2`暂定、= `3`忙碌、= 外出, `4`= 在其他地方工作。</span><span class="sxs-lookup"><span data-stu-id="65596-113">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="65596-114">error</span><span class="sxs-lookup"><span data-stu-id="65596-114">error</span></span> |[<span data-ttu-id="65596-115">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="65596-115">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="65596-116">有关尝试获取用户、通讯组列表或资源的可用性的错误信息。</span><span class="sxs-lookup"><span data-stu-id="65596-116">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="65596-117">scheduleId</span><span class="sxs-lookup"><span data-stu-id="65596-117">scheduleId</span></span> |<span data-ttu-id="65596-118">String</span><span class="sxs-lookup"><span data-stu-id="65596-118">String</span></span> |<span data-ttu-id="65596-119">标识**scheduleInformation**实例的用户、通讯组列表或资源的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="65596-119">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="65596-120">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="65596-120">scheduleItems</span></span> |<span data-ttu-id="65596-121">[scheduleItem](scheduleitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="65596-121">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="65596-122">包含描述用户或资源可用性的项。</span><span class="sxs-lookup"><span data-stu-id="65596-122">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="65596-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="65596-123">workingHours</span></span> |[<span data-ttu-id="65596-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="65596-124">workingHours</span></span>](workinghours.md) |<span data-ttu-id="65596-125">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="65596-125">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="65596-126">这些设置为用户的[mailboxSettings](mailboxsettings.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="65596-126">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="65596-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65596-127">JSON representation</span></span>

<span data-ttu-id="65596-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65596-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
