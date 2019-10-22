---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 4e906a2f7f9d95cd3c3623d1f84c41aedded6cc4
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621585"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="10ed9-104">与会者资源类型</span><span class="sxs-lookup"><span data-stu-id="10ed9-104">attendee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10ed9-105">会议与会者。</span><span class="sxs-lookup"><span data-stu-id="10ed9-105">An event attendee.</span></span> <span data-ttu-id="10ed9-106">这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。</span><span class="sxs-lookup"><span data-stu-id="10ed9-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="10ed9-107">由 [attendeeBase](attendeebase.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="10ed9-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="10ed9-108">属性</span><span class="sxs-lookup"><span data-stu-id="10ed9-108">Properties</span></span>
| <span data-ttu-id="10ed9-109">属性</span><span class="sxs-lookup"><span data-stu-id="10ed9-109">Property</span></span>     | <span data-ttu-id="10ed9-110">类型</span><span class="sxs-lookup"><span data-stu-id="10ed9-110">Type</span></span>   |<span data-ttu-id="10ed9-111">说明</span><span class="sxs-lookup"><span data-stu-id="10ed9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10ed9-112">emailAddress</span><span class="sxs-lookup"><span data-stu-id="10ed9-112">emailAddress</span></span>|[<span data-ttu-id="10ed9-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="10ed9-113">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="10ed9-114">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="10ed9-114">Includes the name and SMTP address of the attendee.</span></span>|
|<span data-ttu-id="10ed9-115">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="10ed9-115">proposedNewTime</span></span>|[<span data-ttu-id="10ed9-116">timeSlot</span><span class="sxs-lookup"><span data-stu-id="10ed9-116">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="10ed9-117">与会者为开始和结束会议请求建议的备用日期/时间。</span><span class="sxs-lookup"><span data-stu-id="10ed9-117">An alternate date/time proposed by the attendee for a meeting request to start and end.</span></span> <span data-ttu-id="10ed9-118">如果与会者尚未建议其他时间，则 GET 事件响应中不包含此属性。</span><span class="sxs-lookup"><span data-stu-id="10ed9-118">If the attendee hasn't proposed another time, then this property is not included in a response of a GET event.</span></span>|
|<span data-ttu-id="10ed9-119">状态</span><span class="sxs-lookup"><span data-stu-id="10ed9-119">status</span></span>|[<span data-ttu-id="10ed9-120">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="10ed9-120">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="10ed9-121">事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。</span><span class="sxs-lookup"><span data-stu-id="10ed9-121">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="10ed9-122">type</span><span class="sxs-lookup"><span data-stu-id="10ed9-122">type</span></span>|<span data-ttu-id="10ed9-123">String</span><span class="sxs-lookup"><span data-stu-id="10ed9-123">String</span></span>|<span data-ttu-id="10ed9-124">与会者类型：`required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="10ed9-124">The attendee type: `required`, `optional`, `resource`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10ed9-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10ed9-125">JSON representation</span></span>

<span data-ttu-id="10ed9-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10ed9-126">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "proposedNewTime"
  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
