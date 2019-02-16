---
title: attendeeDataModel 资源类型
description: 与会者类型。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8659b88cae8b9d2a94177593da40b61363fa23b
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057351"
---
# <a name="attendeedatamodel-resource-type"></a><span data-ttu-id="3d595-103">attendeeDataModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d595-103">attendeeDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d595-104">表示包含在会议中的个人或资源。</span><span class="sxs-lookup"><span data-stu-id="3d595-104">Represents a person or resource who is being included in a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d595-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d595-105">JSON representation</span></span>

<span data-ttu-id="3d595-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d595-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "type"
  ],
  "@odata.type": "microsoft.graph.attendeeDataModel"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="3d595-107">属性</span><span class="sxs-lookup"><span data-stu-id="3d595-107">Properties</span></span>
| <span data-ttu-id="3d595-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d595-108">Property</span></span>     | <span data-ttu-id="3d595-109">类型</span><span class="sxs-lookup"><span data-stu-id="3d595-109">Type</span></span>   |<span data-ttu-id="3d595-110">说明</span><span class="sxs-lookup"><span data-stu-id="3d595-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d595-111">type</span><span class="sxs-lookup"><span data-stu-id="3d595-111">type</span></span>|<span data-ttu-id="3d595-112">attendeeType</span><span class="sxs-lookup"><span data-stu-id="3d595-112">attendeeType</span></span>| <span data-ttu-id="3d595-113">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="3d595-113">The type of attendee.</span></span> <span data-ttu-id="3d595-114">可能的值为: `required`、 `optional`、 `resource`。</span><span class="sxs-lookup"><span data-stu-id="3d595-114">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="3d595-115">目前, 如果与会者是一个人, [findMeetingTimes](../api/user-findmeetingtimes.md)始终认为此人属于该`required`类型。</span><span class="sxs-lookup"><span data-stu-id="3d595-115">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `required` type.</span></span>|
|<span data-ttu-id="3d595-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3d595-116">emailAddress</span></span>|[<span data-ttu-id="3d595-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3d595-117">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="3d595-118">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="3d595-118">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeedatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->