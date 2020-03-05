---
title: attendeeAvailability 资源类型
description: 与会者的可用性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5c01c12f486fd8efeb5a3c9ba3d90776e480bafa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508141"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="faf57-103">attendeeAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="faf57-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="faf57-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="faf57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faf57-105">与会者的可用性。</span><span class="sxs-lookup"><span data-stu-id="faf57-105">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="faf57-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faf57-106">JSON representation</span></span>

<span data-ttu-id="faf57-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faf57-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="faf57-108">属性</span><span class="sxs-lookup"><span data-stu-id="faf57-108">Properties</span></span>
| <span data-ttu-id="faf57-109">属性</span><span class="sxs-lookup"><span data-stu-id="faf57-109">Property</span></span>     | <span data-ttu-id="faf57-110">类型</span><span class="sxs-lookup"><span data-stu-id="faf57-110">Type</span></span>   |<span data-ttu-id="faf57-111">说明</span><span class="sxs-lookup"><span data-stu-id="faf57-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faf57-112">attendee</span><span class="sxs-lookup"><span data-stu-id="faf57-112">attendee</span></span>|[<span data-ttu-id="faf57-113">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="faf57-113">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="faf57-114">电子邮件地址和与会者类型-无论是个人还是资源，如果是个人或资源，是必需的还是可选的。</span><span class="sxs-lookup"><span data-stu-id="faf57-114">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="faf57-115">availability</span><span class="sxs-lookup"><span data-stu-id="faf57-115">availability</span></span>|<span data-ttu-id="faf57-116">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="faf57-116">freeBusyStatus</span></span>| <span data-ttu-id="faf57-p101">与会者的忙/闲状态。可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="faf57-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
