---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
ms.openlocfilehash: b30e054e6d89765d280340b31355403739381c2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844979"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="3e65d-103">attendeeBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e65d-103">attendeeBase resource type</span></span>

> <span data-ttu-id="3e65d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3e65d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e65d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3e65d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e65d-106">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="3e65d-106">The type of attendee.</span></span>

<span data-ttu-id="3e65d-107">由 [recipient](recipient.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="3e65d-107">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e65d-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e65d-108">JSON representation</span></span>

<span data-ttu-id="3e65d-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e65d-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3e65d-110">属性</span><span class="sxs-lookup"><span data-stu-id="3e65d-110">Properties</span></span>
| <span data-ttu-id="3e65d-111">属性</span><span class="sxs-lookup"><span data-stu-id="3e65d-111">Property</span></span>     | <span data-ttu-id="3e65d-112">类型</span><span class="sxs-lookup"><span data-stu-id="3e65d-112">Type</span></span>   |<span data-ttu-id="3e65d-113">说明</span><span class="sxs-lookup"><span data-stu-id="3e65d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e65d-114">type</span><span class="sxs-lookup"><span data-stu-id="3e65d-114">type</span></span>|<span data-ttu-id="3e65d-115">字符串</span><span class="sxs-lookup"><span data-stu-id="3e65d-115">String</span></span>| <span data-ttu-id="3e65d-p102">与会者类型。可取值为：`required`、`optional`、`resource`。目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。</span><span class="sxs-lookup"><span data-stu-id="3e65d-p102">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="3e65d-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3e65d-119">emailAddress</span></span>|[<span data-ttu-id="3e65d-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3e65d-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="3e65d-121">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="3e65d-121">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
