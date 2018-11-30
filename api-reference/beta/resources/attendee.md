---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
ms.openlocfilehash: 7c1a4d5fb483dc722768c9b95885837bdaf6087e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046204"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="fc898-104">与会者资源类型</span><span class="sxs-lookup"><span data-stu-id="fc898-104">attendee resource type</span></span>

> <span data-ttu-id="fc898-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fc898-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc898-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fc898-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc898-107">会议与会者。</span><span class="sxs-lookup"><span data-stu-id="fc898-107">An event attendee.</span></span> <span data-ttu-id="fc898-108">这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。</span><span class="sxs-lookup"><span data-stu-id="fc898-108">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="fc898-109">由 [attendeeBase](attendeebase.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="fc898-109">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fc898-110">属性</span><span class="sxs-lookup"><span data-stu-id="fc898-110">Properties</span></span>
| <span data-ttu-id="fc898-111">属性</span><span class="sxs-lookup"><span data-stu-id="fc898-111">Property</span></span>     | <span data-ttu-id="fc898-112">类型</span><span class="sxs-lookup"><span data-stu-id="fc898-112">Type</span></span>   |<span data-ttu-id="fc898-113">说明</span><span class="sxs-lookup"><span data-stu-id="fc898-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc898-114">状态</span><span class="sxs-lookup"><span data-stu-id="fc898-114">status</span></span>|[<span data-ttu-id="fc898-115">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="fc898-115">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="fc898-116">事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。</span><span class="sxs-lookup"><span data-stu-id="fc898-116">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="fc898-117">类型</span><span class="sxs-lookup"><span data-stu-id="fc898-117">type</span></span>|<span data-ttu-id="fc898-118">String</span><span class="sxs-lookup"><span data-stu-id="fc898-118">String</span></span>|<span data-ttu-id="fc898-119">与会者类型：`required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="fc898-119">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="fc898-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fc898-120">emailAddress</span></span>|[<span data-ttu-id="fc898-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fc898-121">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="fc898-122">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="fc898-122">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc898-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc898-123">JSON representation</span></span>

<span data-ttu-id="fc898-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc898-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->