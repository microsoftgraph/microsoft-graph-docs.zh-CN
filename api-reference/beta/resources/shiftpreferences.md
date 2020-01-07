---
title: shiftPreferences 资源类型
description: 表示计划中用户的已分配班次的可用性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 083b0ad81ffee25d8a03bf5ff38815d2ca0155a8
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952270"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="3b07d-103">shiftPreferences 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b07d-103">shiftPreferences resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b07d-104">表示[计划](schedule.md)中用户的已分配班次的可用性。</span><span class="sxs-lookup"><span data-stu-id="3b07d-104">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3b07d-105">Methods</span><span class="sxs-lookup"><span data-stu-id="3b07d-105">Methods</span></span>

| <span data-ttu-id="3b07d-106">方法</span><span class="sxs-lookup"><span data-stu-id="3b07d-106">Method</span></span>       | <span data-ttu-id="3b07d-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b07d-107">Return Type</span></span> | <span data-ttu-id="3b07d-108">说明</span><span class="sxs-lookup"><span data-stu-id="3b07d-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3b07d-109">Get</span><span class="sxs-lookup"><span data-stu-id="3b07d-109">Get</span></span>](../api/shiftpreferences-get.md) | [<span data-ttu-id="3b07d-110">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="3b07d-110">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="3b07d-111">读取**shiftPreferences**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3b07d-111">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| [<span data-ttu-id="3b07d-112">更新</span><span class="sxs-lookup"><span data-stu-id="3b07d-112">Update</span></span>](../api/shiftpreferences-put.md) | [<span data-ttu-id="3b07d-113">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="3b07d-113">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="3b07d-114">更新**shiftPreferences**对象。</span><span class="sxs-lookup"><span data-stu-id="3b07d-114">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b07d-115">属性</span><span class="sxs-lookup"><span data-stu-id="3b07d-115">Properties</span></span>

|<span data-ttu-id="3b07d-116">属性</span><span class="sxs-lookup"><span data-stu-id="3b07d-116">Property</span></span>          |<span data-ttu-id="3b07d-117">类型</span><span class="sxs-lookup"><span data-stu-id="3b07d-117">Type</span></span>           |<span data-ttu-id="3b07d-118">Description</span><span class="sxs-lookup"><span data-stu-id="3b07d-118">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3b07d-119">id</span><span class="sxs-lookup"><span data-stu-id="3b07d-119">id</span></span> | `Edm.String` | <span data-ttu-id="3b07d-120">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="3b07d-120">The identifier of the entity.</span></span> |
| <span data-ttu-id="3b07d-121">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="3b07d-121">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="3b07d-122">实体的更改键。</span><span class="sxs-lookup"><span data-stu-id="3b07d-122">The change key for the entity.</span></span> |
| <span data-ttu-id="3b07d-123">availability</span><span class="sxs-lookup"><span data-stu-id="3b07d-123">availability</span></span> | <span data-ttu-id="3b07d-124">[shiftAvailability](shiftavailability.md)集合</span><span class="sxs-lookup"><span data-stu-id="3b07d-124">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="3b07d-125">用户计划的工作及其定期模式的可用性。</span><span class="sxs-lookup"><span data-stu-id="3b07d-125">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="3b07d-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b07d-126">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="3b07d-127">创建实体时对应的时间戳。</span><span class="sxs-lookup"><span data-stu-id="3b07d-127">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="3b07d-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b07d-128">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="3b07d-129">上次修改实体时对应的时间戳。</span><span class="sxs-lookup"><span data-stu-id="3b07d-129">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="3b07d-130">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3b07d-130">lastModifiedBy</span></span> | [<span data-ttu-id="3b07d-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="3b07d-131">identitySet</span></span>](identityset.md) | <span data-ttu-id="3b07d-132">上次修改实体的人员的标识。</span><span class="sxs-lookup"><span data-stu-id="3b07d-132">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3b07d-133">关系</span><span class="sxs-lookup"><span data-stu-id="3b07d-133">Relationships</span></span>

<span data-ttu-id="3b07d-134">无。</span><span class="sxs-lookup"><span data-stu-id="3b07d-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b07d-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b07d-135">JSON representation</span></span>

<span data-ttu-id="3b07d-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b07d-136">The following is a JSON representation of the resource.</span></span>

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
