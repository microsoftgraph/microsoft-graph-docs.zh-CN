---
title: attendeeAvailability 资源类型
description: 与会者的可用性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c893b8c14cdb321d435f08c71c50fe43893c76f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003253"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="73b69-103">attendeeAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="73b69-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="73b69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73b69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73b69-105">与会者的可用性。</span><span class="sxs-lookup"><span data-stu-id="73b69-105">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73b69-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73b69-106">JSON representation</span></span>

<span data-ttu-id="73b69-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73b69-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="73b69-108">属性</span><span class="sxs-lookup"><span data-stu-id="73b69-108">Properties</span></span>
| <span data-ttu-id="73b69-109">属性</span><span class="sxs-lookup"><span data-stu-id="73b69-109">Property</span></span>     | <span data-ttu-id="73b69-110">类型</span><span class="sxs-lookup"><span data-stu-id="73b69-110">Type</span></span>   |<span data-ttu-id="73b69-111">说明</span><span class="sxs-lookup"><span data-stu-id="73b69-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73b69-112">attendee</span><span class="sxs-lookup"><span data-stu-id="73b69-112">attendee</span></span>|[<span data-ttu-id="73b69-113">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="73b69-113">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="73b69-114">电子邮件地址和与会者类型-无论是个人还是资源，如果是个人或资源，是必需的还是可选的。</span><span class="sxs-lookup"><span data-stu-id="73b69-114">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="73b69-115">availability</span><span class="sxs-lookup"><span data-stu-id="73b69-115">availability</span></span>|<span data-ttu-id="73b69-116">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="73b69-116">freeBusyStatus</span></span>| <span data-ttu-id="73b69-117">与会者的忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="73b69-117">The availability status of the attendee.</span></span> <span data-ttu-id="73b69-118">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="73b69-118">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

