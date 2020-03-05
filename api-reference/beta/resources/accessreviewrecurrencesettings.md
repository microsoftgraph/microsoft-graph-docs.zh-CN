---
title: accessReviewRecurrenceSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: ''
ms.openlocfilehash: 807be44f256fa3a9080cc3cb458033726aadc107
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508469"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="58444-102">accessReviewRecurrenceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="58444-102">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="58444-103">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="58444-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="58444-104">属性</span><span class="sxs-lookup"><span data-stu-id="58444-104">Properties</span></span>
|<span data-ttu-id="58444-105">属性</span><span class="sxs-lookup"><span data-stu-id="58444-105">Property</span></span>|<span data-ttu-id="58444-106">类型</span><span class="sxs-lookup"><span data-stu-id="58444-106">Type</span></span>|<span data-ttu-id="58444-107">说明</span><span class="sxs-lookup"><span data-stu-id="58444-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="58444-108">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="58444-108">recurrenceType</span></span> | <span data-ttu-id="58444-109">string</span><span class="sxs-lookup"><span data-stu-id="58444-109">string</span></span> |  |
| <span data-ttu-id="58444-110">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="58444-110">recurrenceEndType</span></span> | <span data-ttu-id="58444-111">string</span><span class="sxs-lookup"><span data-stu-id="58444-111">string</span></span> |  |
| <span data-ttu-id="58444-112">durationInDays</span><span class="sxs-lookup"><span data-stu-id="58444-112">durationInDays</span></span> | <span data-ttu-id="58444-113">Int32</span><span class="sxs-lookup"><span data-stu-id="58444-113">Int32</span></span> |  |
| <span data-ttu-id="58444-114">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="58444-114">recurrenceCount</span></span> | <span data-ttu-id="58444-115">Int32</span><span class="sxs-lookup"><span data-stu-id="58444-115">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="58444-116">关系</span><span class="sxs-lookup"><span data-stu-id="58444-116">Relationships</span></span>
<span data-ttu-id="58444-117">无</span><span class="sxs-lookup"><span data-stu-id="58444-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="58444-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58444-118">JSON Representation</span></span>
<span data-ttu-id="58444-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58444-119">Here is a JSON representation of the resource.</span></span>
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



