---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: dfa873daf5b3c5a47e10ab480292ffb11b656b01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974293"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="0667f-103">attendeeBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="0667f-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0667f-104">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="0667f-104">The type of attendee.</span></span>

<span data-ttu-id="0667f-105">由 [recipient](recipient.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="0667f-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0667f-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0667f-106">JSON representation</span></span>

<span data-ttu-id="0667f-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0667f-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0667f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0667f-108">Properties</span></span>
| <span data-ttu-id="0667f-109">属性</span><span class="sxs-lookup"><span data-stu-id="0667f-109">Property</span></span>     | <span data-ttu-id="0667f-110">类型</span><span class="sxs-lookup"><span data-stu-id="0667f-110">Type</span></span>   |<span data-ttu-id="0667f-111">说明</span><span class="sxs-lookup"><span data-stu-id="0667f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0667f-112">type</span><span class="sxs-lookup"><span data-stu-id="0667f-112">type</span></span>|<span data-ttu-id="0667f-113">String</span><span class="sxs-lookup"><span data-stu-id="0667f-113">String</span></span>| <span data-ttu-id="0667f-p101">与会者类型。可取值为：`required`、`optional`、`resource`。目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。</span><span class="sxs-lookup"><span data-stu-id="0667f-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="0667f-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0667f-117">emailAddress</span></span>|[<span data-ttu-id="0667f-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0667f-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="0667f-119">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="0667f-119">Includes the name and SMTP address of the attendee.</span></span>|

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
