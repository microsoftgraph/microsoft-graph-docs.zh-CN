---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: michaelcurnutt
ms.openlocfilehash: 0f2f069cbbff191cefcdc8b735b2847b48a8f2ed
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030780"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="e7bd7-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7bd7-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="e7bd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7bd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7bd7-105">**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="e7bd7-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span> <span data-ttu-id="e7bd7-106">有关订阅进度状态详细信息，请参阅如果我 [的订阅过期，如何？](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="e7bd7-106">For more information on the progression states of a subscription, see [What if my subscription expires?](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)</span></span>

## <a name="properties"></a><span data-ttu-id="e7bd7-107">属性</span><span class="sxs-lookup"><span data-stu-id="e7bd7-107">Properties</span></span>
| <span data-ttu-id="e7bd7-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7bd7-108">Property</span></span>     | <span data-ttu-id="e7bd7-109">类型</span><span class="sxs-lookup"><span data-stu-id="e7bd7-109">Type</span></span>   |<span data-ttu-id="e7bd7-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7bd7-110">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="e7bd7-111">已启用</span><span class="sxs-lookup"><span data-stu-id="e7bd7-111">enabled</span></span>|<span data-ttu-id="e7bd7-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bd7-112">Int32</span></span>| <span data-ttu-id="e7bd7-113">为服务 SKU 的活动订阅启用的单位数。</span><span class="sxs-lookup"><span data-stu-id="e7bd7-113">The number of units that are enabled for the active subscription of the service SKU.</span></span> |
|<span data-ttu-id="e7bd7-114">已挂起</span><span class="sxs-lookup"><span data-stu-id="e7bd7-114">suspended</span></span>|<span data-ttu-id="e7bd7-115">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bd7-115">Int32</span></span>| <span data-ttu-id="e7bd7-116">由于服务 SKU 的订阅已取消而暂停的单位数。</span><span class="sxs-lookup"><span data-stu-id="e7bd7-116">The number of units that are suspended because the subscription of the service SKU has been cancelled.</span></span> <span data-ttu-id="e7bd7-117">无法分配单位，但仍可以在删除之前将其重新激活。</span><span class="sxs-lookup"><span data-stu-id="e7bd7-117">The units cannot be assigned but can still be reactivated before they are deleted.</span></span> |
|<span data-ttu-id="e7bd7-118">警告</span><span class="sxs-lookup"><span data-stu-id="e7bd7-118">warning</span></span>|<span data-ttu-id="e7bd7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bd7-119">Int32</span></span>| <span data-ttu-id="e7bd7-120">警告状态的单位数。</span><span class="sxs-lookup"><span data-stu-id="e7bd7-120">The number of units that are in warning status.</span></span> <span data-ttu-id="e7bd7-121">当服务 SKU 订阅已过期时，客户有一个宽限期来续订其订阅，然后取消订阅 (移动到暂停状态) 。 </span><span class="sxs-lookup"><span data-stu-id="e7bd7-121">When the subscription of the service SKU has expired, the customer has a grace period to renew their subscription before it is cancelled (moved to a **suspended** state).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e7bd7-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7bd7-122">JSON representation</span></span>

<span data-ttu-id="e7bd7-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7bd7-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


