---
title: timeCardBreak 资源类型
description: 表示特定时间卡中断。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 509667ec1fad41f956ee5ee6d6a4371b8d17fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786366"
---
# <a name="timecardbreak-resource-type"></a><span data-ttu-id="821bb-103">timeCardBreak 资源类型</span><span class="sxs-lookup"><span data-stu-id="821bb-103">timeCardBreak resource type</span></span>

<span data-ttu-id="821bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="821bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="821bb-105">表示特定 [timeCard](timecard.md) 中断。</span><span class="sxs-lookup"><span data-stu-id="821bb-105">Represents a specific [timeCard](timecard.md) break.</span></span>

## <a name="properties"></a><span data-ttu-id="821bb-106">属性</span><span class="sxs-lookup"><span data-stu-id="821bb-106">Properties</span></span>
|<span data-ttu-id="821bb-107">属性</span><span class="sxs-lookup"><span data-stu-id="821bb-107">Property</span></span>               |<span data-ttu-id="821bb-108">类型</span><span class="sxs-lookup"><span data-stu-id="821bb-108">Type</span></span>           |<span data-ttu-id="821bb-109">说明</span><span class="sxs-lookup"><span data-stu-id="821bb-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="821bb-110">breakId</span><span class="sxs-lookup"><span data-stu-id="821bb-110">breakId</span></span>                   |`Edm.string`  |<span data-ttu-id="821bb-111">**timeCardBreak** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="821bb-111">ID of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="821bb-112">start</span><span class="sxs-lookup"><span data-stu-id="821bb-112">start</span></span>                 |[<span data-ttu-id="821bb-113">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="821bb-113">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="821bb-114">**timeCardBreak 的开始事件**。</span><span class="sxs-lookup"><span data-stu-id="821bb-114">The start event of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="821bb-115">end</span><span class="sxs-lookup"><span data-stu-id="821bb-115">end</span></span>                   |[<span data-ttu-id="821bb-116">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="821bb-116">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="821bb-117">**timeCardBreak 的开始事件**。</span><span class="sxs-lookup"><span data-stu-id="821bb-117">The start event of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="821bb-118">notes</span><span class="sxs-lookup"><span data-stu-id="821bb-118">notes</span></span>                 |[<span data-ttu-id="821bb-119">itemBody</span><span class="sxs-lookup"><span data-stu-id="821bb-119">itemBody</span></span>](itembody.md)  | <span data-ttu-id="821bb-120">有关 **timeCardBreak 的注释**。</span><span class="sxs-lookup"><span data-stu-id="821bb-120">Notes about the **timeCardBreak**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="821bb-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="821bb-121">JSON representation</span></span>

<span data-ttu-id="821bb-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="821bb-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardBreak"
}-->
```json
{
    "breakId":"string",
    "notes":{
        "content": "string",
        "contentType": "string"
    },
    "start":{
        "dateTime":"String (timestamp)",
        "atApprovedLocation":true,
        "notes":{
            "content": "string",
            "contentType": "text"
        },
    },
    "end":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardBreak resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
