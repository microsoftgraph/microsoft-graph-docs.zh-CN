---
title: accessReviewRecurrenceSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: markwahl-msft
ms.openlocfilehash: 7c45a0b57d869acdb49c5a37f235232c70e8ec6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472234"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="da619-102">accessReviewRecurrenceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="da619-102">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="da619-103">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da619-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="da619-104">属性</span><span class="sxs-lookup"><span data-stu-id="da619-104">Properties</span></span>
|<span data-ttu-id="da619-105">属性</span><span class="sxs-lookup"><span data-stu-id="da619-105">Property</span></span>|<span data-ttu-id="da619-106">类型</span><span class="sxs-lookup"><span data-stu-id="da619-106">Type</span></span>|<span data-ttu-id="da619-107">说明</span><span class="sxs-lookup"><span data-stu-id="da619-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="da619-108">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="da619-108">recurrenceType</span></span> | <span data-ttu-id="da619-109">string</span><span class="sxs-lookup"><span data-stu-id="da619-109">string</span></span> |  |
| <span data-ttu-id="da619-110">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="da619-110">recurrenceEndType</span></span> | <span data-ttu-id="da619-111">string</span><span class="sxs-lookup"><span data-stu-id="da619-111">string</span></span> |  |
| <span data-ttu-id="da619-112">durationInDays</span><span class="sxs-lookup"><span data-stu-id="da619-112">durationInDays</span></span> | <span data-ttu-id="da619-113">Int32</span><span class="sxs-lookup"><span data-stu-id="da619-113">Int32</span></span> |  |
| <span data-ttu-id="da619-114">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="da619-114">recurrenceCount</span></span> | <span data-ttu-id="da619-115">Int32</span><span class="sxs-lookup"><span data-stu-id="da619-115">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="da619-116">关系</span><span class="sxs-lookup"><span data-stu-id="da619-116">Relationships</span></span>
<span data-ttu-id="da619-117">无</span><span class="sxs-lookup"><span data-stu-id="da619-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="da619-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da619-118">JSON Representation</span></span>
<span data-ttu-id="da619-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da619-119">Here is a JSON representation of the resource.</span></span>
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



