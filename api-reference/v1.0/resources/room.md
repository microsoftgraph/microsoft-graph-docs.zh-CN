---
title: 会议室资源类型
description: 指定租户中聊天室的属性。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1a297888d8b469944b5fdbebaa9948db0ba59c97
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059663"
---
# <a name="room-resource-type"></a><span data-ttu-id="c6626-103">会议室资源类型</span><span class="sxs-lookup"><span data-stu-id="c6626-103">room resource type</span></span>

<span data-ttu-id="c6626-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6626-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6626-105">表示租户中的聊天室。</span><span class="sxs-lookup"><span data-stu-id="c6626-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="c6626-106">在 Exchange Online 中，每个会议室都与一个会议室邮箱关联。</span><span class="sxs-lookup"><span data-stu-id="c6626-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="c6626-107">派生自 [位置](place.md)。</span><span class="sxs-lookup"><span data-stu-id="c6626-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c6626-108">方法</span><span class="sxs-lookup"><span data-stu-id="c6626-108">Methods</span></span>

| <span data-ttu-id="c6626-109">方法</span><span class="sxs-lookup"><span data-stu-id="c6626-109">Method</span></span>                              | <span data-ttu-id="c6626-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6626-110">Return Type</span></span>                  | <span data-ttu-id="c6626-111">说明</span><span class="sxs-lookup"><span data-stu-id="c6626-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="c6626-112">列出位置</span><span class="sxs-lookup"><span data-stu-id="c6626-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="c6626-113">所请求的派生位置类型 [的集合](place.md)</span><span class="sxs-lookup"><span data-stu-id="c6626-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="c6626-114">获取租户中定义的指定类型的 **place** 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c6626-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="c6626-115">例如，可以获取租户中特定会议室列表中的所有会议室、所有会议室列表或会议室。</span><span class="sxs-lookup"><span data-stu-id="c6626-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="c6626-116">获取位置</span><span class="sxs-lookup"><span data-stu-id="c6626-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="c6626-117">请求的派生位置 [类型](place.md)</span><span class="sxs-lookup"><span data-stu-id="c6626-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="c6626-118">获取指定位置 **对象（如** 聊天室）的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6626-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6626-119">属性</span><span class="sxs-lookup"><span data-stu-id="c6626-119">Properties</span></span>

| <span data-ttu-id="c6626-120">属性</span><span class="sxs-lookup"><span data-stu-id="c6626-120">Property</span></span>               | <span data-ttu-id="c6626-121">类型</span><span class="sxs-lookup"><span data-stu-id="c6626-121">Type</span></span>                                              | <span data-ttu-id="c6626-122">说明</span><span class="sxs-lookup"><span data-stu-id="c6626-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="c6626-123">address</span><span class="sxs-lookup"><span data-stu-id="c6626-123">address</span></span>                | [<span data-ttu-id="c6626-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c6626-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="c6626-125">房间的街道地址。</span><span class="sxs-lookup"><span data-stu-id="c6626-125">The street address of the room.</span></span> |
| <span data-ttu-id="c6626-126">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="c6626-126">audioDeviceName</span></span>        | <span data-ttu-id="c6626-127">String</span><span class="sxs-lookup"><span data-stu-id="c6626-127">String</span></span>                                            | <span data-ttu-id="c6626-128">指定会议室中的音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="c6626-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="c6626-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="c6626-129">bookingType</span></span>            | [<span data-ttu-id="c6626-130">bookingType</span><span class="sxs-lookup"><span data-stu-id="c6626-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="c6626-131">聊天室的类型。</span><span class="sxs-lookup"><span data-stu-id="c6626-131">Type of room.</span></span> <span data-ttu-id="c6626-132">可能的值是 `standard` ， `reserved` 和 。</span><span class="sxs-lookup"><span data-stu-id="c6626-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="c6626-133">building</span><span class="sxs-lookup"><span data-stu-id="c6626-133">building</span></span>               | <span data-ttu-id="c6626-134">String</span><span class="sxs-lookup"><span data-stu-id="c6626-134">String</span></span>                                            | <span data-ttu-id="c6626-135">指定房间的大楼名称或建筑物编号。</span><span class="sxs-lookup"><span data-stu-id="c6626-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="c6626-136">capacity</span><span class="sxs-lookup"><span data-stu-id="c6626-136">capacity</span></span>               | <span data-ttu-id="c6626-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c6626-137">Int32</span></span>                                             | <span data-ttu-id="c6626-138">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="c6626-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="c6626-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c6626-139">displayName</span></span>            | <span data-ttu-id="c6626-140">String</span><span class="sxs-lookup"><span data-stu-id="c6626-140">String</span></span>                                            | <span data-ttu-id="c6626-141">与聊天室关联的名称。</span><span class="sxs-lookup"><span data-stu-id="c6626-141">The name associated with the room.</span></span> |
| <span data-ttu-id="c6626-142">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="c6626-142">displayDeviceName</span></span>      | <span data-ttu-id="c6626-143">String</span><span class="sxs-lookup"><span data-stu-id="c6626-143">String</span></span>                                            | <span data-ttu-id="c6626-144">指定会议室中的显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="c6626-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="c6626-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c6626-145">emailAddress</span></span>           | <span data-ttu-id="c6626-146">String</span><span class="sxs-lookup"><span data-stu-id="c6626-146">String</span></span>                                            | <span data-ttu-id="c6626-147">会议室的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c6626-147">Email address of the room.</span></span> |
| <span data-ttu-id="c6626-148">floorLabel</span><span class="sxs-lookup"><span data-stu-id="c6626-148">floorLabel</span></span>             | <span data-ttu-id="c6626-149">String</span><span class="sxs-lookup"><span data-stu-id="c6626-149">String</span></span>                                            | <span data-ttu-id="c6626-150">指定楼层的描述性标签，例如 P。</span><span class="sxs-lookup"><span data-stu-id="c6626-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="c6626-151">floorNumber</span><span class="sxs-lookup"><span data-stu-id="c6626-151">floorNumber</span></span>            | <span data-ttu-id="c6626-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c6626-152">Int32</span></span>                                             | <span data-ttu-id="c6626-153">指定房间的楼层。</span><span class="sxs-lookup"><span data-stu-id="c6626-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="c6626-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c6626-154">geoCoordinates</span></span>         | [<span data-ttu-id="c6626-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c6626-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="c6626-156">指定以纬度、经度和（可选）高度坐标表示的会议室位置。</span><span class="sxs-lookup"><span data-stu-id="c6626-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="c6626-157">id</span><span class="sxs-lookup"><span data-stu-id="c6626-157">id</span></span>                     | <span data-ttu-id="c6626-158">String</span><span class="sxs-lookup"><span data-stu-id="c6626-158">String</span></span>                                            | <span data-ttu-id="c6626-159">会议室的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c6626-159">Unique identifier for the room.</span></span> <span data-ttu-id="c6626-160">只读。</span><span class="sxs-lookup"><span data-stu-id="c6626-160">Read-only.</span></span> |
| <span data-ttu-id="c6626-161">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="c6626-161">isWheelChairAccessible</span></span> | <span data-ttu-id="c6626-162">布尔</span><span class="sxs-lookup"><span data-stu-id="c6626-162">Boolean</span></span>                                           | <span data-ttu-id="c6626-163">指定会议室是否可供访问。</span><span class="sxs-lookup"><span data-stu-id="c6626-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="c6626-164">label</span><span class="sxs-lookup"><span data-stu-id="c6626-164">label</span></span>                  | <span data-ttu-id="c6626-165">String</span><span class="sxs-lookup"><span data-stu-id="c6626-165">String</span></span>                                            | <span data-ttu-id="c6626-166">指定会议室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="c6626-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="c6626-167">nickname</span><span class="sxs-lookup"><span data-stu-id="c6626-167">nickname</span></span>               | <span data-ttu-id="c6626-168">String</span><span class="sxs-lookup"><span data-stu-id="c6626-168">String</span></span>                                            | <span data-ttu-id="c6626-169">指定会议室的昵称，例如"conf room"。</span><span class="sxs-lookup"><span data-stu-id="c6626-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="c6626-170">phone</span><span class="sxs-lookup"><span data-stu-id="c6626-170">phone</span></span>                  | <span data-ttu-id="c6626-171">String</span><span class="sxs-lookup"><span data-stu-id="c6626-171">String</span></span>                                            | <span data-ttu-id="c6626-172">会议室的电话号码。</span><span class="sxs-lookup"><span data-stu-id="c6626-172">The phone number of the room.</span></span> |
| <span data-ttu-id="c6626-173">tags</span><span class="sxs-lookup"><span data-stu-id="c6626-173">tags</span></span>                   | <span data-ttu-id="c6626-174">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c6626-174">String collection</span></span>                                 | <span data-ttu-id="c6626-175">指定会议室的其他功能，例如，视图类型或费用类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="c6626-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="c6626-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="c6626-176">videoDeviceName</span></span>        | <span data-ttu-id="c6626-177">String</span><span class="sxs-lookup"><span data-stu-id="c6626-177">String</span></span>                                            | <span data-ttu-id="c6626-178">指定会议室中的视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="c6626-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="c6626-179">bookingType 值</span><span class="sxs-lookup"><span data-stu-id="c6626-179">bookingType values</span></span>

| <span data-ttu-id="c6626-180">值</span><span class="sxs-lookup"><span data-stu-id="c6626-180">Value</span></span>    | <span data-ttu-id="c6626-181">说明</span><span class="sxs-lookup"><span data-stu-id="c6626-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="c6626-182">standard</span><span class="sxs-lookup"><span data-stu-id="c6626-182">standard</span></span> | <span data-ttu-id="c6626-183">会议室可用，可以预订。</span><span class="sxs-lookup"><span data-stu-id="c6626-183">The room is available and can be reserved.</span></span> <span data-ttu-id="c6626-184">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="c6626-184">This is the default value.</span></span> |
| <span data-ttu-id="c6626-185">保留</span><span class="sxs-lookup"><span data-stu-id="c6626-185">reserved</span></span> | <span data-ttu-id="c6626-186">会议室仅在"先到先得"的基础上可用。</span><span class="sxs-lookup"><span data-stu-id="c6626-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="c6626-187">不能保留。</span><span class="sxs-lookup"><span data-stu-id="c6626-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6626-188">关系</span><span class="sxs-lookup"><span data-stu-id="c6626-188">Relationships</span></span>

<span data-ttu-id="c6626-189">无。</span><span class="sxs-lookup"><span data-stu-id="c6626-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6626-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6626-190">JSON representation</span></span>

<span data-ttu-id="c6626-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6626-191">The following is a JSON representation of the resource.</span></span>

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
  "capacity": 1024,
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelChairAccessible": true,
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

