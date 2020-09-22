---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 947b137d3619cca6cc9a6faa8c3f3e761d15fb37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040159"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="51d98-103">attendeeBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="51d98-103">attendeeBase resource type</span></span>

<span data-ttu-id="51d98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51d98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51d98-105">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="51d98-105">The type of attendee.</span></span>

<span data-ttu-id="51d98-106">由 [recipient](recipient.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="51d98-106">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="51d98-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51d98-107">JSON representation</span></span>

<span data-ttu-id="51d98-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51d98-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="51d98-109">属性</span><span class="sxs-lookup"><span data-stu-id="51d98-109">Properties</span></span>
| <span data-ttu-id="51d98-110">属性</span><span class="sxs-lookup"><span data-stu-id="51d98-110">Property</span></span>     | <span data-ttu-id="51d98-111">类型</span><span class="sxs-lookup"><span data-stu-id="51d98-111">Type</span></span>   |<span data-ttu-id="51d98-112">说明</span><span class="sxs-lookup"><span data-stu-id="51d98-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51d98-113">type</span><span class="sxs-lookup"><span data-stu-id="51d98-113">type</span></span>|<span data-ttu-id="51d98-114">String</span><span class="sxs-lookup"><span data-stu-id="51d98-114">String</span></span>| <span data-ttu-id="51d98-p101">与会者类型。可取值为：`required`、`optional`、`resource`。目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。</span><span class="sxs-lookup"><span data-stu-id="51d98-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="51d98-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="51d98-118">emailAddress</span></span>|[<span data-ttu-id="51d98-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="51d98-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="51d98-120">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="51d98-120">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


