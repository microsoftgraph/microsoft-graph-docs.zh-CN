---
title: timeCardEvent 资源类型
description: 表示特定时间卡事件。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a8be7d000b3d55368f7378e9b993b5015b7ef632
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786367"
---
# <a name="timecardevent-resource-type"></a><span data-ttu-id="a962c-103">timeCardEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="a962c-103">timeCardEvent resource type</span></span>

<span data-ttu-id="a962c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a962c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a962c-105">表示特定 [timeCard](timecard.md) 事件。</span><span class="sxs-lookup"><span data-stu-id="a962c-105">Represents a specific [timeCard](timecard.md) event.</span></span>

## <a name="properties"></a><span data-ttu-id="a962c-106">属性</span><span class="sxs-lookup"><span data-stu-id="a962c-106">Properties</span></span>
|<span data-ttu-id="a962c-107">属性</span><span class="sxs-lookup"><span data-stu-id="a962c-107">Property</span></span>               |<span data-ttu-id="a962c-108">类型</span><span class="sxs-lookup"><span data-stu-id="a962c-108">Type</span></span>           |<span data-ttu-id="a962c-109">说明</span><span class="sxs-lookup"><span data-stu-id="a962c-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="a962c-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="a962c-110">dateTime</span></span>                  |`Edm.dateTimeOffset`  |<span data-ttu-id="a962c-111">记录条目的时间。</span><span class="sxs-lookup"><span data-stu-id="a962c-111">The time the entry is recorded.</span></span> |
| <span data-ttu-id="a962c-112">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="a962c-112">atApprovedLocation</span></span> |`Edm.boolean `  |<span data-ttu-id="a962c-113">指示条目是否记录在已批准的位置。</span><span class="sxs-lookup"><span data-stu-id="a962c-113">Indicates whether the entry was recorded at the approved location.</span></span> |
| <span data-ttu-id="a962c-114">notes</span><span class="sxs-lookup"><span data-stu-id="a962c-114">notes</span></span>                 |[<span data-ttu-id="a962c-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="a962c-115">itemBody</span></span>](itembody.md)  | <span data-ttu-id="a962c-116">有关 **timeCardEvent 的注释**。</span><span class="sxs-lookup"><span data-stu-id="a962c-116">Notes about the **timeCardEvent**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a962c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a962c-117">JSON representation</span></span>

<span data-ttu-id="a962c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a962c-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEvent"
}-->
```json
{
   "atApprovedLocation":true,
   "notes":{ "@odata.type":"microsoft.graph.itemBody" }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
