---
title: roomList 资源类型
description: 代表由公司创建的一组聊天室。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f0c56f986663c71d8c6817c0024919e8714af94a
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841253"
---
# <a name="roomlist-resource-type"></a><span data-ttu-id="37db6-103">roomList 资源类型</span><span class="sxs-lookup"><span data-stu-id="37db6-103">roomList resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37db6-104">表示在租户中定义的一组[聊天室](room.md)对象。</span><span class="sxs-lookup"><span data-stu-id="37db6-104">Represents a group of [room](room.md) objects defined in the tenant.</span></span>

<span data-ttu-id="37db6-105">从[原位置](place.md)派生。</span><span class="sxs-lookup"><span data-stu-id="37db6-105">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="37db6-106">方法</span><span class="sxs-lookup"><span data-stu-id="37db6-106">Methods</span></span>

| <span data-ttu-id="37db6-107">方法</span><span class="sxs-lookup"><span data-stu-id="37db6-107">Method</span></span>                              | <span data-ttu-id="37db6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="37db6-108">Return Type</span></span>                  | <span data-ttu-id="37db6-109">说明</span><span class="sxs-lookup"><span data-stu-id="37db6-109">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="37db6-110">列表位置</span><span class="sxs-lookup"><span data-stu-id="37db6-110">List places</span></span>](../api/place-list.md) | <span data-ttu-id="37db6-111">所请求的派生类型的[位置](place.md)的集合</span><span class="sxs-lookup"><span data-stu-id="37db6-111">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="37db6-112">获取在租户中定义的指定类型的**位置**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="37db6-112">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="37db6-113">例如, 您可以获取租户中的所有会议室、所有会议室列表或特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="37db6-113">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>|
| [<span data-ttu-id="37db6-114">获取位置</span><span class="sxs-lookup"><span data-stu-id="37db6-114">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="37db6-115">所请求的派生类型的[位置](place.md)</span><span class="sxs-lookup"><span data-stu-id="37db6-115">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="37db6-116">获取指定的**place**对象的属性和关系, 如会议室列表。</span><span class="sxs-lookup"><span data-stu-id="37db6-116">Get the properties and relationships of the specified **place** object, such as a room list.</span></span> |

## <a name="properties"></a><span data-ttu-id="37db6-117">属性</span><span class="sxs-lookup"><span data-stu-id="37db6-117">Properties</span></span>

| <span data-ttu-id="37db6-118">属性</span><span class="sxs-lookup"><span data-stu-id="37db6-118">Property</span></span>       | <span data-ttu-id="37db6-119">类型</span><span class="sxs-lookup"><span data-stu-id="37db6-119">Type</span></span>                                              | <span data-ttu-id="37db6-120">说明</span><span class="sxs-lookup"><span data-stu-id="37db6-120">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="37db6-121">address</span><span class="sxs-lookup"><span data-stu-id="37db6-121">address</span></span>        | [<span data-ttu-id="37db6-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="37db6-122">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="37db6-123">会议室列表的街道地址。</span><span class="sxs-lookup"><span data-stu-id="37db6-123">The street address of the room list.</span></span> |
| <span data-ttu-id="37db6-124">displayName</span><span class="sxs-lookup"><span data-stu-id="37db6-124">displayName</span></span>    | <span data-ttu-id="37db6-125">字符串</span><span class="sxs-lookup"><span data-stu-id="37db6-125">String</span></span>                                            | <span data-ttu-id="37db6-126">与会议室列表关联的名称。</span><span class="sxs-lookup"><span data-stu-id="37db6-126">The name associated with the room list.</span></span> |
| <span data-ttu-id="37db6-127">emailAddress</span><span class="sxs-lookup"><span data-stu-id="37db6-127">emailAddress</span></span>   | <span data-ttu-id="37db6-128">String</span><span class="sxs-lookup"><span data-stu-id="37db6-128">String</span></span>                                            | <span data-ttu-id="37db6-129">会议室列表的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="37db6-129">The email address of the room list.</span></span> |
| <span data-ttu-id="37db6-130">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="37db6-130">geoCoordinates</span></span> | [<span data-ttu-id="37db6-131">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="37db6-131">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="37db6-132">指定纬度、经度和 (可选) 海拔高度坐标中的 roomlist 位置。</span><span class="sxs-lookup"><span data-stu-id="37db6-132">Specifies the roomlist location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="37db6-133">id</span><span class="sxs-lookup"><span data-stu-id="37db6-133">id</span></span>             | <span data-ttu-id="37db6-134">String</span><span class="sxs-lookup"><span data-stu-id="37db6-134">String</span></span>                                            | <span data-ttu-id="37db6-135">会议室列表的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37db6-135">Unique identifier for the room list.</span></span> <span data-ttu-id="37db6-136">只读。</span><span class="sxs-lookup"><span data-stu-id="37db6-136">Read-only.</span></span> |
| <span data-ttu-id="37db6-137">phone</span><span class="sxs-lookup"><span data-stu-id="37db6-137">phone</span></span>          | <span data-ttu-id="37db6-138">String</span><span class="sxs-lookup"><span data-stu-id="37db6-138">String</span></span>                                            | <span data-ttu-id="37db6-139">会议室列表的电话号码。</span><span class="sxs-lookup"><span data-stu-id="37db6-139">The phone number of the room list.</span></span> |

## <a name="relationships"></a><span data-ttu-id="37db6-140">关系</span><span class="sxs-lookup"><span data-stu-id="37db6-140">Relationships</span></span>

| <span data-ttu-id="37db6-141">关系</span><span class="sxs-lookup"><span data-stu-id="37db6-141">Relationship</span></span> | <span data-ttu-id="37db6-142">类型</span><span class="sxs-lookup"><span data-stu-id="37db6-142">Type</span></span>                         | <span data-ttu-id="37db6-143">说明</span><span class="sxs-lookup"><span data-stu-id="37db6-143">Description</span></span>          |
|:-------------|:-----------------------------|:---------------------|
| <span data-ttu-id="37db6-144">所属</span><span class="sxs-lookup"><span data-stu-id="37db6-144">rooms</span></span>        | <span data-ttu-id="37db6-145">[place](place.md)集合</span><span class="sxs-lookup"><span data-stu-id="37db6-145">[place](place.md) collection</span></span> | <span data-ttu-id="37db6-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="37db6-p103">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37db6-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37db6-148">JSON representation</span></span>

<span data-ttu-id="37db6-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37db6-149">The following is a JSON representation of the resource.</span></span>

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
