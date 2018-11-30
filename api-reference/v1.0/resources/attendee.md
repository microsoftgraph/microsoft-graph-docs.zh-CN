---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
ms.openlocfilehash: 7c9040b563840c22eec1dd7456892fc7ff83ee4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011745"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="ebe87-104">与会者资源类型</span><span class="sxs-lookup"><span data-stu-id="ebe87-104">attendee resource type</span></span>

<span data-ttu-id="ebe87-105">会议与会者。</span><span class="sxs-lookup"><span data-stu-id="ebe87-105">An event attendee.</span></span> <span data-ttu-id="ebe87-106">这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。</span><span class="sxs-lookup"><span data-stu-id="ebe87-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="ebe87-107">由 [attendeeBase](attendeebase.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="ebe87-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ebe87-108">属性</span><span class="sxs-lookup"><span data-stu-id="ebe87-108">Properties</span></span>
| <span data-ttu-id="ebe87-109">属性</span><span class="sxs-lookup"><span data-stu-id="ebe87-109">Property</span></span>     | <span data-ttu-id="ebe87-110">类型</span><span class="sxs-lookup"><span data-stu-id="ebe87-110">Type</span></span>   |<span data-ttu-id="ebe87-111">说明</span><span class="sxs-lookup"><span data-stu-id="ebe87-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebe87-112">状态</span><span class="sxs-lookup"><span data-stu-id="ebe87-112">status</span></span>|[<span data-ttu-id="ebe87-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="ebe87-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="ebe87-114">事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。</span><span class="sxs-lookup"><span data-stu-id="ebe87-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="ebe87-115">类型</span><span class="sxs-lookup"><span data-stu-id="ebe87-115">type</span></span>|<span data-ttu-id="ebe87-116">String</span><span class="sxs-lookup"><span data-stu-id="ebe87-116">String</span></span>|<span data-ttu-id="ebe87-117">与会者类型：`required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="ebe87-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="ebe87-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ebe87-118">emailAddress</span></span>|[<span data-ttu-id="ebe87-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ebe87-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ebe87-120">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="ebe87-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebe87-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebe87-121">JSON representation</span></span>

<span data-ttu-id="ebe87-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebe87-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
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