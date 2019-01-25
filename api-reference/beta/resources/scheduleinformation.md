---
title: scheduleInformation 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: e84505ee2f30a5b7b52e9d5b589b8bb24d9a4c95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521906"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="1eb95-104">scheduleInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1eb95-104">scheduleInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="1eb95-105">在指定的时间段代表用户、 通讯组列表或资源的可用性。</span><span class="sxs-lookup"><span data-stu-id="1eb95-105">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="1eb95-106">属性</span><span class="sxs-lookup"><span data-stu-id="1eb95-106">Properties</span></span>
| <span data-ttu-id="1eb95-107">属性</span><span class="sxs-lookup"><span data-stu-id="1eb95-107">Property</span></span>     | <span data-ttu-id="1eb95-108">类型</span><span class="sxs-lookup"><span data-stu-id="1eb95-108">Type</span></span>   |<span data-ttu-id="1eb95-109">说明</span><span class="sxs-lookup"><span data-stu-id="1eb95-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1eb95-110">availabilityView</span><span class="sxs-lookup"><span data-stu-id="1eb95-110">availabilityView</span></span> |<span data-ttu-id="1eb95-111">String</span><span class="sxs-lookup"><span data-stu-id="1eb95-111">String</span></span> |<span data-ttu-id="1eb95-112">表示的合并的视图中的所有项目的可用性的`scheduleItems`。</span><span class="sxs-lookup"><span data-stu-id="1eb95-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="1eb95-113">视图包含的时间段。</span><span class="sxs-lookup"><span data-stu-id="1eb95-113">The view consists of time slots.</span></span> <span data-ttu-id="1eb95-114">指示期间每个时间段的可用性：`0`免费 = `1`= 暂定、 `2`= 忙`3`= 外出、 `4`= 其他地方工作。</span><span class="sxs-lookup"><span data-stu-id="1eb95-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="1eb95-115">error</span><span class="sxs-lookup"><span data-stu-id="1eb95-115">error</span></span> |[<span data-ttu-id="1eb95-116">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="1eb95-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="1eb95-117">从尝试获取用户、 通讯组列表或资源的可用性信息的错误。</span><span class="sxs-lookup"><span data-stu-id="1eb95-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="1eb95-118">scheduleId</span><span class="sxs-lookup"><span data-stu-id="1eb95-118">scheduleId</span></span> |<span data-ttu-id="1eb95-119">String</span><span class="sxs-lookup"><span data-stu-id="1eb95-119">String</span></span> |<span data-ttu-id="1eb95-120">用户、 通讯组列表或资源，标识实例**scheduleInformation**SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="1eb95-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="1eb95-121">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="1eb95-121">scheduleItems</span></span> |<span data-ttu-id="1eb95-122">[scheduleItem](scheduleitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="1eb95-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="1eb95-123">包含描述的用户或资源的可用性的项。</span><span class="sxs-lookup"><span data-stu-id="1eb95-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="1eb95-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="1eb95-124">workingHours</span></span> |[<span data-ttu-id="1eb95-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="1eb95-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="1eb95-126">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="1eb95-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="1eb95-127">这些设置用户的[mailboxSettings](mailboxsettings.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="1eb95-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1eb95-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1eb95-128">JSON representation</span></span>

<span data-ttu-id="1eb95-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1eb95-129">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
