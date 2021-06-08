---
title: timeCardEntry 资源类型
description: 表示特定考勤卡条目。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d09b324b4d43765f05de789129021e2eb1f24789
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786382"
---
# <a name="timecardentry-resource-type"></a><span data-ttu-id="1aecd-103">timeCardEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="1aecd-103">timeCardEntry resource type</span></span>

<span data-ttu-id="1aecd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1aecd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aecd-105">表示特定 [timeCard](timecard.md) 条目。</span><span class="sxs-lookup"><span data-stu-id="1aecd-105">Represents a specific [timeCard](timecard.md) entry.</span></span>

## <a name="properties"></a><span data-ttu-id="1aecd-106">属性</span><span class="sxs-lookup"><span data-stu-id="1aecd-106">Properties</span></span>
|<span data-ttu-id="1aecd-107">属性</span><span class="sxs-lookup"><span data-stu-id="1aecd-107">Property</span></span>               |<span data-ttu-id="1aecd-108">类型</span><span class="sxs-lookup"><span data-stu-id="1aecd-108">Type</span></span>           |<span data-ttu-id="1aecd-109">说明</span><span class="sxs-lookup"><span data-stu-id="1aecd-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="1aecd-110">clockInEvent</span><span class="sxs-lookup"><span data-stu-id="1aecd-110">clockInEvent</span></span>       |[<span data-ttu-id="1aecd-111">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="1aecd-111">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="1aecd-112">timeCard 的 **时钟事件**。</span><span class="sxs-lookup"><span data-stu-id="1aecd-112">The clock-in event of the **timeCard**.</span></span>|
| <span data-ttu-id="1aecd-113">clockOutEvent</span><span class="sxs-lookup"><span data-stu-id="1aecd-113">clockOutEvent</span></span>                 |[<span data-ttu-id="1aecd-114">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="1aecd-114">timeCardEvent</span></span>](timecardevent.md)  |<span data-ttu-id="1aecd-115">timeCard 的 **时钟出事件**。</span><span class="sxs-lookup"><span data-stu-id="1aecd-115">The clock-out event of the **timeCard**.</span></span> |
| <span data-ttu-id="1aecd-116">breaks</span><span class="sxs-lookup"><span data-stu-id="1aecd-116">breaks</span></span>    |<span data-ttu-id="1aecd-117">[timeCardBreak](timecardbreak.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1aecd-117">[timeCardBreak](timecardbreak.md) collection</span></span>    |<span data-ttu-id="1aecd-118">与 **timeCard** 关联的中断列表。</span><span class="sxs-lookup"><span data-stu-id="1aecd-118">The list of breaks associated with the **timeCard**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1aecd-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1aecd-119">JSON representation</span></span>

<span data-ttu-id="1aecd-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aecd-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEntry"
}-->
```json
{
   "clockInEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "clockOutEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "string",
             "contentType": "text"
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
   ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timecardentry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
