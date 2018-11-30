---
title: scheduleInformation 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: 0b7bbd861a044b28cd22603fd0ccc27d20f46fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044801"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="f1997-104">scheduleInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1997-104">scheduleInformation resource type</span></span>

 > <span data-ttu-id="f1997-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f1997-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1997-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1997-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f1997-107">在指定的时间段代表用户、 通讯组列表或资源的可用性。</span><span class="sxs-lookup"><span data-stu-id="f1997-107">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="f1997-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1997-108">Properties</span></span>
| <span data-ttu-id="f1997-109">属性</span><span class="sxs-lookup"><span data-stu-id="f1997-109">Property</span></span>     | <span data-ttu-id="f1997-110">类型</span><span class="sxs-lookup"><span data-stu-id="f1997-110">Type</span></span>   |<span data-ttu-id="f1997-111">说明</span><span class="sxs-lookup"><span data-stu-id="f1997-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1997-112">availabilityView</span><span class="sxs-lookup"><span data-stu-id="f1997-112">availabilityView</span></span> |<span data-ttu-id="f1997-113">字符串</span><span class="sxs-lookup"><span data-stu-id="f1997-113">String</span></span> |<span data-ttu-id="f1997-114">表示的合并的视图中的所有项目的可用性的`scheduleItems`。</span><span class="sxs-lookup"><span data-stu-id="f1997-114">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="f1997-115">视图包含的时间段。</span><span class="sxs-lookup"><span data-stu-id="f1997-115">The view consists of time slots.</span></span> <span data-ttu-id="f1997-116">指示期间每个时间段的可用性：`0`免费 = `1`= 暂定、 `2`= 忙`3`= 外出、 `4`= 其他地方工作。</span><span class="sxs-lookup"><span data-stu-id="f1997-116">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="f1997-117">error</span><span class="sxs-lookup"><span data-stu-id="f1997-117">error</span></span> |[<span data-ttu-id="f1997-118">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="f1997-118">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="f1997-119">从尝试获取用户、 通讯组列表或资源的可用性信息的错误。</span><span class="sxs-lookup"><span data-stu-id="f1997-119">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="f1997-120">scheduleId</span><span class="sxs-lookup"><span data-stu-id="f1997-120">scheduleId</span></span> |<span data-ttu-id="f1997-121">字符串</span><span class="sxs-lookup"><span data-stu-id="f1997-121">String</span></span> |<span data-ttu-id="f1997-122">用户、 通讯组列表或资源，标识实例**scheduleInformation**SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="f1997-122">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="f1997-123">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="f1997-123">scheduleItems</span></span> |<span data-ttu-id="f1997-124">[scheduleItem](scheduleitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1997-124">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="f1997-125">包含描述的用户或资源的可用性的项。</span><span class="sxs-lookup"><span data-stu-id="f1997-125">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="f1997-126">workingHours</span><span class="sxs-lookup"><span data-stu-id="f1997-126">workingHours</span></span> |[<span data-ttu-id="f1997-127">workingHours</span><span class="sxs-lookup"><span data-stu-id="f1997-127">workingHours</span></span>](workinghours.md) |<span data-ttu-id="f1997-128">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="f1997-128">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="f1997-129">这些设置用户的[mailboxSettings](mailboxsettings.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="f1997-129">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f1997-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1997-130">JSON representation</span></span>

<span data-ttu-id="f1997-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1997-131">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->