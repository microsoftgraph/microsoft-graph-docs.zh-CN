---
title: accessReviewRecurrenceSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: markwahl-msft
ms.openlocfilehash: e629bbe5affbf2f21b7c4041e62a3df68785dacc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024580"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="b26dd-102">accessReviewRecurrenceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b26dd-102">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="b26dd-103">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b26dd-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="b26dd-104">属性</span><span class="sxs-lookup"><span data-stu-id="b26dd-104">Properties</span></span>
|<span data-ttu-id="b26dd-105">属性</span><span class="sxs-lookup"><span data-stu-id="b26dd-105">Property</span></span>|<span data-ttu-id="b26dd-106">类型</span><span class="sxs-lookup"><span data-stu-id="b26dd-106">Type</span></span>|<span data-ttu-id="b26dd-107">说明</span><span class="sxs-lookup"><span data-stu-id="b26dd-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="b26dd-108">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="b26dd-108">recurrenceType</span></span> | <span data-ttu-id="b26dd-109">string</span><span class="sxs-lookup"><span data-stu-id="b26dd-109">string</span></span> |  |
| <span data-ttu-id="b26dd-110">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="b26dd-110">recurrenceEndType</span></span> | <span data-ttu-id="b26dd-111">string</span><span class="sxs-lookup"><span data-stu-id="b26dd-111">string</span></span> |  |
| <span data-ttu-id="b26dd-112">durationInDays</span><span class="sxs-lookup"><span data-stu-id="b26dd-112">durationInDays</span></span> | <span data-ttu-id="b26dd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b26dd-113">Int32</span></span> |  |
| <span data-ttu-id="b26dd-114">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="b26dd-114">recurrenceCount</span></span> | <span data-ttu-id="b26dd-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b26dd-115">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="b26dd-116">关系</span><span class="sxs-lookup"><span data-stu-id="b26dd-116">Relationships</span></span>
<span data-ttu-id="b26dd-117">无</span><span class="sxs-lookup"><span data-stu-id="b26dd-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b26dd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b26dd-118">JSON Representation</span></span>
<span data-ttu-id="b26dd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b26dd-119">Here is a JSON representation of the resource.</span></span>
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





