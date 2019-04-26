---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
ms.openlocfilehash: a0095a2076cd09bee2d4b934bac29cd030924ec1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328527"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="b0a53-103">attendeeBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0a53-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0a53-104">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="b0a53-104">The type of attendee.</span></span>

<span data-ttu-id="b0a53-105">由 [recipient](recipient.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="b0a53-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0a53-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0a53-106">JSON representation</span></span>

<span data-ttu-id="b0a53-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0a53-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b0a53-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0a53-108">Properties</span></span>
| <span data-ttu-id="b0a53-109">属性</span><span class="sxs-lookup"><span data-stu-id="b0a53-109">Property</span></span>     | <span data-ttu-id="b0a53-110">类型</span><span class="sxs-lookup"><span data-stu-id="b0a53-110">Type</span></span>   |<span data-ttu-id="b0a53-111">说明</span><span class="sxs-lookup"><span data-stu-id="b0a53-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0a53-112">type</span><span class="sxs-lookup"><span data-stu-id="b0a53-112">type</span></span>|<span data-ttu-id="b0a53-113">String</span><span class="sxs-lookup"><span data-stu-id="b0a53-113">String</span></span>| <span data-ttu-id="b0a53-p101">与会者类型。可取值为：`required`、`optional`、`resource`。目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。</span><span class="sxs-lookup"><span data-stu-id="b0a53-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="b0a53-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b0a53-117">emailAddress</span></span>|[<span data-ttu-id="b0a53-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b0a53-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="b0a53-119">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="b0a53-119">Includes the name and SMTP address of the attendee.</span></span>|

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
