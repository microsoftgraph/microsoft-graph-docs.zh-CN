---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
ms.openlocfilehash: 6ec80f5505cb3dd742a2690ebb3cd5374635770d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572736"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="da6aa-103">attendeeBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="da6aa-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da6aa-104">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="da6aa-104">The type of attendee.</span></span>

<span data-ttu-id="da6aa-105">由 [recipient](recipient.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="da6aa-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="da6aa-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da6aa-106">JSON representation</span></span>

<span data-ttu-id="da6aa-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da6aa-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="da6aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="da6aa-108">Properties</span></span>
| <span data-ttu-id="da6aa-109">属性</span><span class="sxs-lookup"><span data-stu-id="da6aa-109">Property</span></span>     | <span data-ttu-id="da6aa-110">类型</span><span class="sxs-lookup"><span data-stu-id="da6aa-110">Type</span></span>   |<span data-ttu-id="da6aa-111">说明</span><span class="sxs-lookup"><span data-stu-id="da6aa-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da6aa-112">type</span><span class="sxs-lookup"><span data-stu-id="da6aa-112">type</span></span>|<span data-ttu-id="da6aa-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="da6aa-113">attendeeType</span></span>| <span data-ttu-id="da6aa-114">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="da6aa-114">The type of attendee.</span></span> <span data-ttu-id="da6aa-115">可能的值为： `required`， `optional`， `resource`。</span><span class="sxs-lookup"><span data-stu-id="da6aa-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="da6aa-116">当前如果参与者的人员， [findMeetingTimes](../api/user-findmeetingtimes.md)总是将此人为`Required`类型。</span><span class="sxs-lookup"><span data-stu-id="da6aa-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="da6aa-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="da6aa-117">emailAddress</span></span>|[<span data-ttu-id="da6aa-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="da6aa-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="da6aa-119">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="da6aa-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
