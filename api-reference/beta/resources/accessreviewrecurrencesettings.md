---
title: accessReviewRecurrenceSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: ''
ms.openlocfilehash: 2bf71fe1c715eb96e98b0caf7720cc0d637ee33b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974520"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="22724-102">accessReviewRecurrenceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="22724-102">accessReviewRecurrenceSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="22724-103">属性</span><span class="sxs-lookup"><span data-stu-id="22724-103">Properties</span></span>
|<span data-ttu-id="22724-104">属性</span><span class="sxs-lookup"><span data-stu-id="22724-104">Property</span></span>|<span data-ttu-id="22724-105">类型</span><span class="sxs-lookup"><span data-stu-id="22724-105">Type</span></span>|<span data-ttu-id="22724-106">说明</span><span class="sxs-lookup"><span data-stu-id="22724-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="22724-107">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="22724-107">recurrenceType</span></span> | <span data-ttu-id="22724-108">string</span><span class="sxs-lookup"><span data-stu-id="22724-108">string</span></span> |  |
| <span data-ttu-id="22724-109">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="22724-109">recurrenceEndType</span></span> | <span data-ttu-id="22724-110">string</span><span class="sxs-lookup"><span data-stu-id="22724-110">string</span></span> |  |
| <span data-ttu-id="22724-111">durationInDays</span><span class="sxs-lookup"><span data-stu-id="22724-111">durationInDays</span></span> | <span data-ttu-id="22724-112">Int32</span><span class="sxs-lookup"><span data-stu-id="22724-112">Int32</span></span> |  |
| <span data-ttu-id="22724-113">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="22724-113">recurrenceCount</span></span> | <span data-ttu-id="22724-114">Int32</span><span class="sxs-lookup"><span data-stu-id="22724-114">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="22724-115">关系</span><span class="sxs-lookup"><span data-stu-id="22724-115">Relationships</span></span>
<span data-ttu-id="22724-116">无</span><span class="sxs-lookup"><span data-stu-id="22724-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="22724-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22724-117">JSON Representation</span></span>
<span data-ttu-id="22724-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22724-118">Here is a JSON representation of the resource.</span></span>
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



