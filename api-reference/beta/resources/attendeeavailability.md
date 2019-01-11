---
title: attendeeAvailability 资源类型
description: 与会者的类型和忙/闲状态。
localization_priority: Normal
ms.openlocfilehash: a00fe38e678c6a51cd252b823a7d2651e531d20a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820466"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="ea6ed-103">attendeeAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea6ed-103">attendeeAvailability resource type</span></span>

> <span data-ttu-id="ea6ed-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea6ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea6ed-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea6ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ea6ed-106">与会者的类型和忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="ea6ed-106">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea6ed-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea6ed-107">JSON representation</span></span>

<span data-ttu-id="ea6ed-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea6ed-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="ea6ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="ea6ed-109">Properties</span></span>
| <span data-ttu-id="ea6ed-110">属性</span><span class="sxs-lookup"><span data-stu-id="ea6ed-110">Property</span></span>     | <span data-ttu-id="ea6ed-111">类型</span><span class="sxs-lookup"><span data-stu-id="ea6ed-111">Type</span></span>   |<span data-ttu-id="ea6ed-112">说明</span><span class="sxs-lookup"><span data-stu-id="ea6ed-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea6ed-113">attendee</span><span class="sxs-lookup"><span data-stu-id="ea6ed-113">attendee</span></span>|[<span data-ttu-id="ea6ed-114">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="ea6ed-114">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="ea6ed-115">与会者类型，即是人员还是资源；如果是人员，是必需还是可选。</span><span class="sxs-lookup"><span data-stu-id="ea6ed-115">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="ea6ed-116">availability</span><span class="sxs-lookup"><span data-stu-id="ea6ed-116">availability</span></span>|<span data-ttu-id="ea6ed-117">字符串</span><span class="sxs-lookup"><span data-stu-id="ea6ed-117">String</span></span>| <span data-ttu-id="ea6ed-p102">与会者的忙/闲状态。可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="ea6ed-p102">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
