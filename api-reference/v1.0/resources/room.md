---
title: 会议室资源类型
description: 指定租户中聊天室的属性。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 14067f71ae338ae0da026c98d6732fc2ae4eaf57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094174"
---
# <a name="room-resource-type"></a><span data-ttu-id="8f634-103">会议室资源类型</span><span class="sxs-lookup"><span data-stu-id="8f634-103">room resource type</span></span>

<span data-ttu-id="8f634-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f634-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f634-105">表示租户中的会议室。</span><span class="sxs-lookup"><span data-stu-id="8f634-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="8f634-106">在 Exchange Online 中，每个会议室都与一个会议室邮箱相关联。</span><span class="sxs-lookup"><span data-stu-id="8f634-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="8f634-107">从 [原位置](place.md)派生。</span><span class="sxs-lookup"><span data-stu-id="8f634-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8f634-108">方法</span><span class="sxs-lookup"><span data-stu-id="8f634-108">Methods</span></span>

| <span data-ttu-id="8f634-109">方法</span><span class="sxs-lookup"><span data-stu-id="8f634-109">Method</span></span>                              | <span data-ttu-id="8f634-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f634-110">Return Type</span></span>                  | <span data-ttu-id="8f634-111">说明</span><span class="sxs-lookup"><span data-stu-id="8f634-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="8f634-112">列表位置</span><span class="sxs-lookup"><span data-stu-id="8f634-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="8f634-113">所请求的派生类型的[位置](place.md)的集合</span><span class="sxs-lookup"><span data-stu-id="8f634-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="8f634-114">获取在租户中定义的指定类型的 **位置** 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="8f634-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="8f634-115">例如，您可以获取租户中的所有会议室、所有会议室列表或特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="8f634-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="8f634-116">获取位置</span><span class="sxs-lookup"><span data-stu-id="8f634-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="8f634-117">所请求的派生类型的 [位置](place.md)</span><span class="sxs-lookup"><span data-stu-id="8f634-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="8f634-118">获取指定的 **place** 对象（例如会议室）的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8f634-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f634-119">属性</span><span class="sxs-lookup"><span data-stu-id="8f634-119">Properties</span></span>

| <span data-ttu-id="8f634-120">属性</span><span class="sxs-lookup"><span data-stu-id="8f634-120">Property</span></span>               | <span data-ttu-id="8f634-121">类型</span><span class="sxs-lookup"><span data-stu-id="8f634-121">Type</span></span>                                              | <span data-ttu-id="8f634-122">说明</span><span class="sxs-lookup"><span data-stu-id="8f634-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="8f634-123">address</span><span class="sxs-lookup"><span data-stu-id="8f634-123">address</span></span>                | [<span data-ttu-id="8f634-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="8f634-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="8f634-125">会议室的街道地址。</span><span class="sxs-lookup"><span data-stu-id="8f634-125">The street address of the room.</span></span> |
| <span data-ttu-id="8f634-126">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="8f634-126">audioDeviceName</span></span>        | <span data-ttu-id="8f634-127">String</span><span class="sxs-lookup"><span data-stu-id="8f634-127">String</span></span>                                            | <span data-ttu-id="8f634-128">指定会议室中音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="8f634-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="8f634-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="8f634-129">bookingType</span></span>            | [<span data-ttu-id="8f634-130">bookingType</span><span class="sxs-lookup"><span data-stu-id="8f634-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="8f634-131">会议室的类型。</span><span class="sxs-lookup"><span data-stu-id="8f634-131">Type of room.</span></span> <span data-ttu-id="8f634-132">可能的值为 `standard` 和 `reserved` 。</span><span class="sxs-lookup"><span data-stu-id="8f634-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="8f634-133">幢</span><span class="sxs-lookup"><span data-stu-id="8f634-133">building</span></span>               | <span data-ttu-id="8f634-134">String</span><span class="sxs-lookup"><span data-stu-id="8f634-134">String</span></span>                                            | <span data-ttu-id="8f634-135">指定聊天室所在的建筑物名称或楼号。</span><span class="sxs-lookup"><span data-stu-id="8f634-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="8f634-136">能够</span><span class="sxs-lookup"><span data-stu-id="8f634-136">capacity</span></span>               | <span data-ttu-id="8f634-137">String</span><span class="sxs-lookup"><span data-stu-id="8f634-137">String</span></span>                                            | <span data-ttu-id="8f634-138">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="8f634-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="8f634-139">displayName</span><span class="sxs-lookup"><span data-stu-id="8f634-139">displayName</span></span>            | <span data-ttu-id="8f634-140">String</span><span class="sxs-lookup"><span data-stu-id="8f634-140">String</span></span>                                            | <span data-ttu-id="8f634-141">与聊天室关联的名称。</span><span class="sxs-lookup"><span data-stu-id="8f634-141">The name associated with the room.</span></span> |
| <span data-ttu-id="8f634-142">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="8f634-142">displayDeviceName</span></span>      | <span data-ttu-id="8f634-143">String</span><span class="sxs-lookup"><span data-stu-id="8f634-143">String</span></span>                                            | <span data-ttu-id="8f634-144">指定聊天室中显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="8f634-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="8f634-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8f634-145">emailAddress</span></span>           | <span data-ttu-id="8f634-146">String</span><span class="sxs-lookup"><span data-stu-id="8f634-146">String</span></span>                                            | <span data-ttu-id="8f634-147">聊天室的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8f634-147">Email address of the room.</span></span> |
| <span data-ttu-id="8f634-148">floorLabel</span><span class="sxs-lookup"><span data-stu-id="8f634-148">floorLabel</span></span>             | <span data-ttu-id="8f634-149">String</span><span class="sxs-lookup"><span data-stu-id="8f634-149">String</span></span>                                            | <span data-ttu-id="8f634-150">指定基底的描述性标签，例如 P。</span><span class="sxs-lookup"><span data-stu-id="8f634-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="8f634-151">floorNumber</span><span class="sxs-lookup"><span data-stu-id="8f634-151">floorNumber</span></span>            | <span data-ttu-id="8f634-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8f634-152">Int32</span></span>                                             | <span data-ttu-id="8f634-153">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="8f634-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="8f634-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="8f634-154">geoCoordinates</span></span>         | [<span data-ttu-id="8f634-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="8f634-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="8f634-156">指定纬度、经度和（可选）海拔坐标中的会议室位置。</span><span class="sxs-lookup"><span data-stu-id="8f634-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="8f634-157">id</span><span class="sxs-lookup"><span data-stu-id="8f634-157">id</span></span>                     | <span data-ttu-id="8f634-158">String</span><span class="sxs-lookup"><span data-stu-id="8f634-158">String</span></span>                                            | <span data-ttu-id="8f634-159">聊天室的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f634-159">Unique identifier for the room.</span></span> <span data-ttu-id="8f634-160">只读。</span><span class="sxs-lookup"><span data-stu-id="8f634-160">Read-only.</span></span> |
| <span data-ttu-id="8f634-161">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="8f634-161">isWheelchairAccessible</span></span> | <span data-ttu-id="8f634-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f634-162">Boolean</span></span>                                           | <span data-ttu-id="8f634-163">指定会议室是否 wheelchair 可访问。</span><span class="sxs-lookup"><span data-stu-id="8f634-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="8f634-164">label</span><span class="sxs-lookup"><span data-stu-id="8f634-164">label</span></span>                  | <span data-ttu-id="8f634-165">String</span><span class="sxs-lookup"><span data-stu-id="8f634-165">String</span></span>                                            | <span data-ttu-id="8f634-166">指定聊天室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="8f634-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="8f634-167">昵称</span><span class="sxs-lookup"><span data-stu-id="8f634-167">nickname</span></span>               | <span data-ttu-id="8f634-168">String</span><span class="sxs-lookup"><span data-stu-id="8f634-168">String</span></span>                                            | <span data-ttu-id="8f634-169">指定聊天室的昵称，例如 "会议室"。</span><span class="sxs-lookup"><span data-stu-id="8f634-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="8f634-170">phone</span><span class="sxs-lookup"><span data-stu-id="8f634-170">phone</span></span>                  | <span data-ttu-id="8f634-171">String</span><span class="sxs-lookup"><span data-stu-id="8f634-171">String</span></span>                                            | <span data-ttu-id="8f634-172">会议室的电话号码。</span><span class="sxs-lookup"><span data-stu-id="8f634-172">The phone number of the room.</span></span> |
| <span data-ttu-id="8f634-173">标记</span><span class="sxs-lookup"><span data-stu-id="8f634-173">tags</span></span>                   | <span data-ttu-id="8f634-174">String collection</span><span class="sxs-lookup"><span data-stu-id="8f634-174">String collection</span></span>                                 | <span data-ttu-id="8f634-175">指定会议室的其他功能，例如，视图类型或家具类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="8f634-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="8f634-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="8f634-176">videoDeviceName</span></span>        | <span data-ttu-id="8f634-177">String</span><span class="sxs-lookup"><span data-stu-id="8f634-177">String</span></span>                                            | <span data-ttu-id="8f634-178">指定聊天室中视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="8f634-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="8f634-179">bookingType 值</span><span class="sxs-lookup"><span data-stu-id="8f634-179">bookingType values</span></span>

| <span data-ttu-id="8f634-180">值</span><span class="sxs-lookup"><span data-stu-id="8f634-180">Value</span></span>    | <span data-ttu-id="8f634-181">说明</span><span class="sxs-lookup"><span data-stu-id="8f634-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="8f634-182">普通</span><span class="sxs-lookup"><span data-stu-id="8f634-182">standard</span></span> | <span data-ttu-id="8f634-183">会议室可用且可以保留。</span><span class="sxs-lookup"><span data-stu-id="8f634-183">The room is available and can be reserved.</span></span> <span data-ttu-id="8f634-184">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="8f634-184">This is the default value.</span></span> |
| <span data-ttu-id="8f634-185">保留</span><span class="sxs-lookup"><span data-stu-id="8f634-185">reserved</span></span> | <span data-ttu-id="8f634-186">会议室仅在首次推出时才可用。</span><span class="sxs-lookup"><span data-stu-id="8f634-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="8f634-187">无法保留。</span><span class="sxs-lookup"><span data-stu-id="8f634-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f634-188">关系</span><span class="sxs-lookup"><span data-stu-id="8f634-188">Relationships</span></span>

<span data-ttu-id="8f634-189">无。</span><span class="sxs-lookup"><span data-stu-id="8f634-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f634-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f634-190">JSON representation</span></span>

<span data-ttu-id="8f634-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f634-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "String",
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelchairAccessible": true,
  "label": "String",
  "nickname": "String",
  "phone": "String",
  "tags": ["String"],
  "videoDeviceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "room resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

