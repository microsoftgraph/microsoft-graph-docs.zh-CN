---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cadb1ca6d2ab1168c3c7f9ff2b182b57112bfb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532091"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="020c6-104">与会者资源类型</span><span class="sxs-lookup"><span data-stu-id="020c6-104">attendee resource type</span></span>

<span data-ttu-id="020c6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="020c6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="020c6-106">会议与会者。</span><span class="sxs-lookup"><span data-stu-id="020c6-106">An event attendee.</span></span> <span data-ttu-id="020c6-107">这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。</span><span class="sxs-lookup"><span data-stu-id="020c6-107">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="020c6-108">由 [attendeeBase](attendeebase.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="020c6-108">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="020c6-109">属性</span><span class="sxs-lookup"><span data-stu-id="020c6-109">Properties</span></span>
| <span data-ttu-id="020c6-110">属性</span><span class="sxs-lookup"><span data-stu-id="020c6-110">Property</span></span>     | <span data-ttu-id="020c6-111">类型</span><span class="sxs-lookup"><span data-stu-id="020c6-111">Type</span></span>   |<span data-ttu-id="020c6-112">说明</span><span class="sxs-lookup"><span data-stu-id="020c6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="020c6-113">状态</span><span class="sxs-lookup"><span data-stu-id="020c6-113">status</span></span>|[<span data-ttu-id="020c6-114">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="020c6-114">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="020c6-115">事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。</span><span class="sxs-lookup"><span data-stu-id="020c6-115">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="020c6-116">type</span><span class="sxs-lookup"><span data-stu-id="020c6-116">type</span></span>|<span data-ttu-id="020c6-117">字符串</span><span class="sxs-lookup"><span data-stu-id="020c6-117">String</span></span>|<span data-ttu-id="020c6-118">与会者类型：`required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="020c6-118">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="020c6-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="020c6-119">emailAddress</span></span>|[<span data-ttu-id="020c6-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="020c6-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="020c6-121">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="020c6-121">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="020c6-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="020c6-122">JSON representation</span></span>

<span data-ttu-id="020c6-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="020c6-123">Here is a JSON representation of the resource</span></span>

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
