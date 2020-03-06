---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a7eaf030413e576721bd672fc63111a62742c163
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532072"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="88ae8-103">attendeeBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="88ae8-103">attendeeBase resource type</span></span>

<span data-ttu-id="88ae8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ae8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88ae8-105">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="88ae8-105">The type of attendee.</span></span>

<span data-ttu-id="88ae8-106">由 [recipient](recipient.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="88ae8-106">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="88ae8-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88ae8-107">JSON representation</span></span>

<span data-ttu-id="88ae8-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88ae8-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="88ae8-109">属性</span><span class="sxs-lookup"><span data-stu-id="88ae8-109">Properties</span></span>
| <span data-ttu-id="88ae8-110">属性</span><span class="sxs-lookup"><span data-stu-id="88ae8-110">Property</span></span>     | <span data-ttu-id="88ae8-111">类型</span><span class="sxs-lookup"><span data-stu-id="88ae8-111">Type</span></span>   |<span data-ttu-id="88ae8-112">说明</span><span class="sxs-lookup"><span data-stu-id="88ae8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88ae8-113">类型</span><span class="sxs-lookup"><span data-stu-id="88ae8-113">type</span></span>|<span data-ttu-id="88ae8-114">attendeeType</span><span class="sxs-lookup"><span data-stu-id="88ae8-114">attendeeType</span></span>| <span data-ttu-id="88ae8-115">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="88ae8-115">The type of attendee.</span></span> <span data-ttu-id="88ae8-116">可能的值包括 `required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="88ae8-116">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="88ae8-117">目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。</span><span class="sxs-lookup"><span data-stu-id="88ae8-117">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="88ae8-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="88ae8-118">emailAddress</span></span>|[<span data-ttu-id="88ae8-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="88ae8-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="88ae8-120">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="88ae8-120">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
