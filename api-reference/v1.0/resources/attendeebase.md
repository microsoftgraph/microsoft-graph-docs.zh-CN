---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 154584a91fc8844e2745d5198773157c4dfe26d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033108"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="26cdc-103">attendeeBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="26cdc-103">attendeeBase resource type</span></span>

<span data-ttu-id="26cdc-104">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="26cdc-104">The type of attendee.</span></span>

<span data-ttu-id="26cdc-105">由 [recipient](recipient.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="26cdc-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="26cdc-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26cdc-106">JSON representation</span></span>

<span data-ttu-id="26cdc-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26cdc-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="26cdc-108">属性</span><span class="sxs-lookup"><span data-stu-id="26cdc-108">Properties</span></span>
| <span data-ttu-id="26cdc-109">属性</span><span class="sxs-lookup"><span data-stu-id="26cdc-109">Property</span></span>     | <span data-ttu-id="26cdc-110">类型</span><span class="sxs-lookup"><span data-stu-id="26cdc-110">Type</span></span>   |<span data-ttu-id="26cdc-111">说明</span><span class="sxs-lookup"><span data-stu-id="26cdc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26cdc-112">类型</span><span class="sxs-lookup"><span data-stu-id="26cdc-112">type</span></span>|<span data-ttu-id="26cdc-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="26cdc-113">attendeeType</span></span>| <span data-ttu-id="26cdc-114">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="26cdc-114">The type of attendee.</span></span> <span data-ttu-id="26cdc-115">可能的值包括 `required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="26cdc-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="26cdc-116">目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。</span><span class="sxs-lookup"><span data-stu-id="26cdc-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="26cdc-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="26cdc-117">emailAddress</span></span>|[<span data-ttu-id="26cdc-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="26cdc-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="26cdc-119">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="26cdc-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
