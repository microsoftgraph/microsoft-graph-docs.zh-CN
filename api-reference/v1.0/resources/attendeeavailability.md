---
title: attendeeAvailability 资源类型
description: 与会者的可用性。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9c69925ee64dd3c39b7edb59a6416d0ddc5b533c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474461"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="fb03e-103">attendeeAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb03e-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="fb03e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb03e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb03e-105">与会者的可用性。</span><span class="sxs-lookup"><span data-stu-id="fb03e-105">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb03e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb03e-106">JSON representation</span></span>

<span data-ttu-id="fb03e-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb03e-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="fb03e-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb03e-108">Properties</span></span>
| <span data-ttu-id="fb03e-109">属性</span><span class="sxs-lookup"><span data-stu-id="fb03e-109">Property</span></span>     | <span data-ttu-id="fb03e-110">类型</span><span class="sxs-lookup"><span data-stu-id="fb03e-110">Type</span></span>   |<span data-ttu-id="fb03e-111">说明</span><span class="sxs-lookup"><span data-stu-id="fb03e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb03e-112">attendee</span><span class="sxs-lookup"><span data-stu-id="fb03e-112">attendee</span></span>|[<span data-ttu-id="fb03e-113">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="fb03e-113">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="fb03e-114">与会者的电子邮件地址和类型 - 无论是人员还是资源，如果是人员，是必需还是可选。</span><span class="sxs-lookup"><span data-stu-id="fb03e-114">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="fb03e-115">availability</span><span class="sxs-lookup"><span data-stu-id="fb03e-115">availability</span></span>|<span data-ttu-id="fb03e-116">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="fb03e-116">freeBusyStatus</span></span>| <span data-ttu-id="fb03e-117">与会者的忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="fb03e-117">The availability status of the attendee.</span></span> <span data-ttu-id="fb03e-118">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="fb03e-118">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

