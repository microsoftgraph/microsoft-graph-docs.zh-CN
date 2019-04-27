---
title: accessReviewRecurrenceSettings 资源类型
description: ''
localization_priority: Normal
ms.openlocfilehash: 1a5235639209830d36cf69c027cfd309fab09c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348349"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="89770-102">accessReviewRecurrenceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="89770-102">accessReviewRecurrenceSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="89770-103">属性</span><span class="sxs-lookup"><span data-stu-id="89770-103">Properties</span></span>
|<span data-ttu-id="89770-104">属性</span><span class="sxs-lookup"><span data-stu-id="89770-104">Property</span></span>|<span data-ttu-id="89770-105">类型</span><span class="sxs-lookup"><span data-stu-id="89770-105">Type</span></span>|<span data-ttu-id="89770-106">说明</span><span class="sxs-lookup"><span data-stu-id="89770-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="89770-107">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="89770-107">recurrenceType</span></span> | <span data-ttu-id="89770-108">string</span><span class="sxs-lookup"><span data-stu-id="89770-108">string</span></span> |  |
| <span data-ttu-id="89770-109">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="89770-109">recurrenceEndType</span></span> | <span data-ttu-id="89770-110">string</span><span class="sxs-lookup"><span data-stu-id="89770-110">string</span></span> |  |
| <span data-ttu-id="89770-111">durationInDays</span><span class="sxs-lookup"><span data-stu-id="89770-111">durationInDays</span></span> | <span data-ttu-id="89770-112">Int32</span><span class="sxs-lookup"><span data-stu-id="89770-112">Int32</span></span> |  |
| <span data-ttu-id="89770-113">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="89770-113">recurrenceCount</span></span> | <span data-ttu-id="89770-114">Int32</span><span class="sxs-lookup"><span data-stu-id="89770-114">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="89770-115">关系</span><span class="sxs-lookup"><span data-stu-id="89770-115">Relationships</span></span>
<span data-ttu-id="89770-116">无</span><span class="sxs-lookup"><span data-stu-id="89770-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89770-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89770-117">JSON Representation</span></span>
<span data-ttu-id="89770-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89770-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
``` json
{
    "recurrenceType":"string",
    "recurrenceEndType":"string",
    "durationInDays":"Int32",
    "recurrenceCount":"Int32"
}
```



