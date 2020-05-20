---
title: roomList 资源类型
description: 代表由公司创建的一组聊天室。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3aa89075b93f34ad565d210bee3dff2bfd1ffe81
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290565"
---
# <a name="roomlist-resource-type"></a><span data-ttu-id="5385f-103">roomList 资源类型</span><span class="sxs-lookup"><span data-stu-id="5385f-103">roomList resource type</span></span>

<span data-ttu-id="5385f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5385f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5385f-105">表示在租户中定义的一组[聊天室](room.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5385f-105">Represents a group of [room](room.md) objects defined in the tenant.</span></span>

<span data-ttu-id="5385f-106">从[原位置](place.md)派生。</span><span class="sxs-lookup"><span data-stu-id="5385f-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5385f-107">Methods</span><span class="sxs-lookup"><span data-stu-id="5385f-107">Methods</span></span>

| <span data-ttu-id="5385f-108">方法</span><span class="sxs-lookup"><span data-stu-id="5385f-108">Method</span></span>                              | <span data-ttu-id="5385f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5385f-109">Return Type</span></span>                  | <span data-ttu-id="5385f-110">说明</span><span class="sxs-lookup"><span data-stu-id="5385f-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="5385f-111">列表位置</span><span class="sxs-lookup"><span data-stu-id="5385f-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="5385f-112">所请求的派生类型的[位置](place.md)的集合</span><span class="sxs-lookup"><span data-stu-id="5385f-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="5385f-113">获取在租户中定义的指定类型的**位置**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5385f-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="5385f-114">例如，您可以获取租户中的所有会议室、所有会议室列表或特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="5385f-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>|
| [<span data-ttu-id="5385f-115">获取位置</span><span class="sxs-lookup"><span data-stu-id="5385f-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="5385f-116">所请求的派生类型的[位置](place.md)</span><span class="sxs-lookup"><span data-stu-id="5385f-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="5385f-117">获取指定的**place**对象的属性和关系，如会议室列表。</span><span class="sxs-lookup"><span data-stu-id="5385f-117">Get the properties and relationships of the specified **place** object, such as a room list.</span></span> |

## <a name="properties"></a><span data-ttu-id="5385f-118">属性</span><span class="sxs-lookup"><span data-stu-id="5385f-118">Properties</span></span>

| <span data-ttu-id="5385f-119">属性</span><span class="sxs-lookup"><span data-stu-id="5385f-119">Property</span></span>       | <span data-ttu-id="5385f-120">类型</span><span class="sxs-lookup"><span data-stu-id="5385f-120">Type</span></span>                                              | <span data-ttu-id="5385f-121">说明</span><span class="sxs-lookup"><span data-stu-id="5385f-121">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="5385f-122">address</span><span class="sxs-lookup"><span data-stu-id="5385f-122">address</span></span>        | [<span data-ttu-id="5385f-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5385f-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="5385f-124">会议室列表的街道地址。</span><span class="sxs-lookup"><span data-stu-id="5385f-124">The street address of the room list.</span></span> |
| <span data-ttu-id="5385f-125">displayName</span><span class="sxs-lookup"><span data-stu-id="5385f-125">displayName</span></span>    | <span data-ttu-id="5385f-126">字符串</span><span class="sxs-lookup"><span data-stu-id="5385f-126">String</span></span>                                            | <span data-ttu-id="5385f-127">与会议室列表关联的名称。</span><span class="sxs-lookup"><span data-stu-id="5385f-127">The name associated with the room list.</span></span> |
| <span data-ttu-id="5385f-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5385f-128">emailAddress</span></span>   | <span data-ttu-id="5385f-129">String</span><span class="sxs-lookup"><span data-stu-id="5385f-129">String</span></span>                                            | <span data-ttu-id="5385f-130">会议室列表的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5385f-130">The email address of the room list.</span></span> |
| <span data-ttu-id="5385f-131">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="5385f-131">geoCoordinates</span></span> | [<span data-ttu-id="5385f-132">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="5385f-132">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="5385f-133">指定纬度、经度和（可选）海拔高度坐标中的 roomlist 位置。</span><span class="sxs-lookup"><span data-stu-id="5385f-133">Specifies the roomlist location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="5385f-134">id</span><span class="sxs-lookup"><span data-stu-id="5385f-134">id</span></span>             | <span data-ttu-id="5385f-135">String</span><span class="sxs-lookup"><span data-stu-id="5385f-135">String</span></span>                                            | <span data-ttu-id="5385f-136">会议室列表的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5385f-136">Unique identifier for the room list.</span></span> <span data-ttu-id="5385f-137">只读。</span><span class="sxs-lookup"><span data-stu-id="5385f-137">Read-only.</span></span> |
| <span data-ttu-id="5385f-138">phone</span><span class="sxs-lookup"><span data-stu-id="5385f-138">phone</span></span>          | <span data-ttu-id="5385f-139">String</span><span class="sxs-lookup"><span data-stu-id="5385f-139">String</span></span>                                            | <span data-ttu-id="5385f-140">会议室列表的电话号码。</span><span class="sxs-lookup"><span data-stu-id="5385f-140">The phone number of the room list.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5385f-141">关系</span><span class="sxs-lookup"><span data-stu-id="5385f-141">Relationships</span></span>

| <span data-ttu-id="5385f-142">关系</span><span class="sxs-lookup"><span data-stu-id="5385f-142">Relationship</span></span> | <span data-ttu-id="5385f-143">类型</span><span class="sxs-lookup"><span data-stu-id="5385f-143">Type</span></span>                         | <span data-ttu-id="5385f-144">Description</span><span class="sxs-lookup"><span data-stu-id="5385f-144">Description</span></span>          |
|:-------------|:-----------------------------|:---------------------|
| <span data-ttu-id="5385f-145">所属</span><span class="sxs-lookup"><span data-stu-id="5385f-145">rooms</span></span>        | <span data-ttu-id="5385f-146">[place](place.md)集合</span><span class="sxs-lookup"><span data-stu-id="5385f-146">[place](place.md) collection</span></span> | <span data-ttu-id="5385f-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="5385f-p103">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5385f-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5385f-149">JSON representation</span></span>

<span data-ttu-id="5385f-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5385f-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roomList"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "emailAddress": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "phone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roomList resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
