---
title: shiftPreferences 资源类型
description: 表示计划中用户的已分配班次的可用性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d35f77e7d048adb0b0bb49604423bbe2ff53031c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058028"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="1d2be-103">shiftPreferences 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d2be-103">shiftPreferences resource type</span></span>

<span data-ttu-id="1d2be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d2be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d2be-105">表示 [计划](schedule.md)中用户的已分配班次的可用性。</span><span class="sxs-lookup"><span data-stu-id="1d2be-105">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1d2be-106">方法</span><span class="sxs-lookup"><span data-stu-id="1d2be-106">Methods</span></span>

| <span data-ttu-id="1d2be-107">方法</span><span class="sxs-lookup"><span data-stu-id="1d2be-107">Method</span></span>       | <span data-ttu-id="1d2be-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d2be-108">Return Type</span></span> | <span data-ttu-id="1d2be-109">说明</span><span class="sxs-lookup"><span data-stu-id="1d2be-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1d2be-110">Get</span><span class="sxs-lookup"><span data-stu-id="1d2be-110">Get</span></span>](../api/shiftpreferences-get.md) | [<span data-ttu-id="1d2be-111">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="1d2be-111">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="1d2be-112">读取 **shiftPreferences** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d2be-112">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| [<span data-ttu-id="1d2be-113">更新</span><span class="sxs-lookup"><span data-stu-id="1d2be-113">Update</span></span>](../api/shiftpreferences-put.md) | [<span data-ttu-id="1d2be-114">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="1d2be-114">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="1d2be-115">更新 **shiftPreferences** 对象。</span><span class="sxs-lookup"><span data-stu-id="1d2be-115">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d2be-116">属性</span><span class="sxs-lookup"><span data-stu-id="1d2be-116">Properties</span></span>

|<span data-ttu-id="1d2be-117">属性</span><span class="sxs-lookup"><span data-stu-id="1d2be-117">Property</span></span>          |<span data-ttu-id="1d2be-118">类型</span><span class="sxs-lookup"><span data-stu-id="1d2be-118">Type</span></span>           |<span data-ttu-id="1d2be-119">说明</span><span class="sxs-lookup"><span data-stu-id="1d2be-119">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1d2be-120">id</span><span class="sxs-lookup"><span data-stu-id="1d2be-120">id</span></span> | `Edm.String` | <span data-ttu-id="1d2be-121">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="1d2be-121">The identifier of the entity.</span></span> |
| <span data-ttu-id="1d2be-122">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="1d2be-122">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="1d2be-123">实体的更改键。</span><span class="sxs-lookup"><span data-stu-id="1d2be-123">The change key for the entity.</span></span> |
| <span data-ttu-id="1d2be-124">availability</span><span class="sxs-lookup"><span data-stu-id="1d2be-124">availability</span></span> | <span data-ttu-id="1d2be-125">[shiftAvailability](shiftavailability.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d2be-125">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="1d2be-126">用户计划的工作及其定期模式的可用性。</span><span class="sxs-lookup"><span data-stu-id="1d2be-126">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="1d2be-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d2be-127">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="1d2be-128">创建实体时对应的时间戳。</span><span class="sxs-lookup"><span data-stu-id="1d2be-128">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="1d2be-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d2be-129">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="1d2be-130">上次修改实体时对应的时间戳。</span><span class="sxs-lookup"><span data-stu-id="1d2be-130">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="1d2be-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1d2be-131">lastModifiedBy</span></span> | [<span data-ttu-id="1d2be-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="1d2be-132">identitySet</span></span>](identityset.md) | <span data-ttu-id="1d2be-133">上次修改实体的人员的标识。</span><span class="sxs-lookup"><span data-stu-id="1d2be-133">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1d2be-134">关系</span><span class="sxs-lookup"><span data-stu-id="1d2be-134">Relationships</span></span>

<span data-ttu-id="1d2be-135">无。</span><span class="sxs-lookup"><span data-stu-id="1d2be-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d2be-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d2be-136">JSON representation</span></span>

<span data-ttu-id="1d2be-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d2be-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftPreferences",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "availability": [{"@odata.type": "microsoft.graph.shiftAvailability"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


