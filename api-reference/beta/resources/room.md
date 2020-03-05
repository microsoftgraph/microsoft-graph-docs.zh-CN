---
title: 会议室资源类型
description: 指定租户中聊天室的属性。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e23d8a873abb0de5a086350b3748f9e40d7e12ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521038"
---
# <a name="room-resource-type"></a><span data-ttu-id="08cb5-103">会议室资源类型</span><span class="sxs-lookup"><span data-stu-id="08cb5-103">room resource type</span></span>

<span data-ttu-id="08cb5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="08cb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08cb5-105">表示租户中的会议室。</span><span class="sxs-lookup"><span data-stu-id="08cb5-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="08cb5-106">在 Exchange Online 中，每个会议室都与一个会议室邮箱相关联。</span><span class="sxs-lookup"><span data-stu-id="08cb5-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="08cb5-107">从[原位置](place.md)派生。</span><span class="sxs-lookup"><span data-stu-id="08cb5-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="08cb5-108">方法</span><span class="sxs-lookup"><span data-stu-id="08cb5-108">Methods</span></span>

| <span data-ttu-id="08cb5-109">方法</span><span class="sxs-lookup"><span data-stu-id="08cb5-109">Method</span></span>                              | <span data-ttu-id="08cb5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="08cb5-110">Return Type</span></span>                  | <span data-ttu-id="08cb5-111">说明</span><span class="sxs-lookup"><span data-stu-id="08cb5-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="08cb5-112">列表位置</span><span class="sxs-lookup"><span data-stu-id="08cb5-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="08cb5-113">所请求的派生类型的[位置](place.md)的集合</span><span class="sxs-lookup"><span data-stu-id="08cb5-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="08cb5-114">获取在租户中定义的指定类型的**位置**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="08cb5-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="08cb5-115">例如，您可以获取租户中的所有会议室、所有会议室列表或特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="08cb5-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="08cb5-116">获取位置</span><span class="sxs-lookup"><span data-stu-id="08cb5-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="08cb5-117">所请求的派生类型的[位置](place.md)</span><span class="sxs-lookup"><span data-stu-id="08cb5-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="08cb5-118">获取指定的**place**对象（例如会议室）的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="08cb5-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="08cb5-119">属性</span><span class="sxs-lookup"><span data-stu-id="08cb5-119">Properties</span></span>

| <span data-ttu-id="08cb5-120">属性</span><span class="sxs-lookup"><span data-stu-id="08cb5-120">Property</span></span>               | <span data-ttu-id="08cb5-121">类型</span><span class="sxs-lookup"><span data-stu-id="08cb5-121">Type</span></span>                                              | <span data-ttu-id="08cb5-122">说明</span><span class="sxs-lookup"><span data-stu-id="08cb5-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="08cb5-123">address</span><span class="sxs-lookup"><span data-stu-id="08cb5-123">address</span></span>                | [<span data-ttu-id="08cb5-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="08cb5-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="08cb5-125">会议室的街道地址。</span><span class="sxs-lookup"><span data-stu-id="08cb5-125">The street address of the room.</span></span> |
| <span data-ttu-id="08cb5-126">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="08cb5-126">audioDeviceName</span></span>        | <span data-ttu-id="08cb5-127">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-127">String</span></span>                                            | <span data-ttu-id="08cb5-128">指定会议室中音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="08cb5-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="08cb5-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="08cb5-129">bookingType</span></span>            | [<span data-ttu-id="08cb5-130">bookingType</span><span class="sxs-lookup"><span data-stu-id="08cb5-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="08cb5-131">会议室的类型。</span><span class="sxs-lookup"><span data-stu-id="08cb5-131">Type of room.</span></span> <span data-ttu-id="08cb5-132">可能的值`standard`为和`reserved`。</span><span class="sxs-lookup"><span data-stu-id="08cb5-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="08cb5-133">幢</span><span class="sxs-lookup"><span data-stu-id="08cb5-133">building</span></span>               | <span data-ttu-id="08cb5-134">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-134">String</span></span>                                            | <span data-ttu-id="08cb5-135">指定聊天室所在的建筑物名称或楼号。</span><span class="sxs-lookup"><span data-stu-id="08cb5-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="08cb5-136">能够</span><span class="sxs-lookup"><span data-stu-id="08cb5-136">capacity</span></span>               | <span data-ttu-id="08cb5-137">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-137">String</span></span>                                            | <span data-ttu-id="08cb5-138">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="08cb5-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="08cb5-139">displayName</span><span class="sxs-lookup"><span data-stu-id="08cb5-139">displayName</span></span>            | <span data-ttu-id="08cb5-140">字符串</span><span class="sxs-lookup"><span data-stu-id="08cb5-140">String</span></span>                                            | <span data-ttu-id="08cb5-141">与聊天室关联的名称。</span><span class="sxs-lookup"><span data-stu-id="08cb5-141">The name associated with the room.</span></span> |
| <span data-ttu-id="08cb5-142">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="08cb5-142">displayDeviceName</span></span>      | <span data-ttu-id="08cb5-143">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-143">String</span></span>                                            | <span data-ttu-id="08cb5-144">指定聊天室中显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="08cb5-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="08cb5-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="08cb5-145">emailAddress</span></span>           | <span data-ttu-id="08cb5-146">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-146">String</span></span>                                            | <span data-ttu-id="08cb5-147">聊天室的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="08cb5-147">Email address of the room.</span></span> |
| <span data-ttu-id="08cb5-148">floorLabel</span><span class="sxs-lookup"><span data-stu-id="08cb5-148">floorLabel</span></span>             | <span data-ttu-id="08cb5-149">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-149">String</span></span>                                            | <span data-ttu-id="08cb5-150">指定基底的描述性标签，例如 P。</span><span class="sxs-lookup"><span data-stu-id="08cb5-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="08cb5-151">floorNumber</span><span class="sxs-lookup"><span data-stu-id="08cb5-151">floorNumber</span></span>            | <span data-ttu-id="08cb5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="08cb5-152">Int32</span></span>                                             | <span data-ttu-id="08cb5-153">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="08cb5-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="08cb5-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="08cb5-154">geoCoordinates</span></span>         | [<span data-ttu-id="08cb5-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="08cb5-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="08cb5-156">指定纬度、经度和（可选）海拔坐标中的会议室位置。</span><span class="sxs-lookup"><span data-stu-id="08cb5-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="08cb5-157">id</span><span class="sxs-lookup"><span data-stu-id="08cb5-157">id</span></span>                     | <span data-ttu-id="08cb5-158">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-158">String</span></span>                                            | <span data-ttu-id="08cb5-159">聊天室的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="08cb5-159">Unique identifier for the room.</span></span> <span data-ttu-id="08cb5-160">只读。</span><span class="sxs-lookup"><span data-stu-id="08cb5-160">Read-only.</span></span> |
| <span data-ttu-id="08cb5-161">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="08cb5-161">isWheelchairAccessible</span></span> | <span data-ttu-id="08cb5-162">布尔</span><span class="sxs-lookup"><span data-stu-id="08cb5-162">Boolean</span></span>                                           | <span data-ttu-id="08cb5-163">指定会议室是否 wheelchair 可访问。</span><span class="sxs-lookup"><span data-stu-id="08cb5-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="08cb5-164">label</span><span class="sxs-lookup"><span data-stu-id="08cb5-164">label</span></span>                  | <span data-ttu-id="08cb5-165">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-165">String</span></span>                                            | <span data-ttu-id="08cb5-166">指定聊天室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="08cb5-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="08cb5-167">昵称</span><span class="sxs-lookup"><span data-stu-id="08cb5-167">nickname</span></span>               | <span data-ttu-id="08cb5-168">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-168">String</span></span>                                            | <span data-ttu-id="08cb5-169">指定聊天室的昵称，例如 "会议室"。</span><span class="sxs-lookup"><span data-stu-id="08cb5-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="08cb5-170">phone</span><span class="sxs-lookup"><span data-stu-id="08cb5-170">phone</span></span>                  | <span data-ttu-id="08cb5-171">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-171">String</span></span>                                            | <span data-ttu-id="08cb5-172">会议室的电话号码。</span><span class="sxs-lookup"><span data-stu-id="08cb5-172">The phone number of the room.</span></span> |
| <span data-ttu-id="08cb5-173">标记</span><span class="sxs-lookup"><span data-stu-id="08cb5-173">tags</span></span>                   | <span data-ttu-id="08cb5-174">String 集合</span><span class="sxs-lookup"><span data-stu-id="08cb5-174">String collection</span></span>                                 | <span data-ttu-id="08cb5-175">指定会议室的其他功能，例如，视图类型或家具类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="08cb5-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="08cb5-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="08cb5-176">videoDeviceName</span></span>        | <span data-ttu-id="08cb5-177">String</span><span class="sxs-lookup"><span data-stu-id="08cb5-177">String</span></span>                                            | <span data-ttu-id="08cb5-178">指定聊天室中视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="08cb5-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="08cb5-179">bookingType 值</span><span class="sxs-lookup"><span data-stu-id="08cb5-179">bookingType values</span></span>

| <span data-ttu-id="08cb5-180">值</span><span class="sxs-lookup"><span data-stu-id="08cb5-180">Value</span></span>    | <span data-ttu-id="08cb5-181">说明</span><span class="sxs-lookup"><span data-stu-id="08cb5-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="08cb5-182">普通</span><span class="sxs-lookup"><span data-stu-id="08cb5-182">standard</span></span> | <span data-ttu-id="08cb5-183">可以根据此 cmdlet 中的其他设置保留该会议室。</span><span class="sxs-lookup"><span data-stu-id="08cb5-183">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="08cb5-184">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="08cb5-184">This is the default value.</span></span> |
| <span data-ttu-id="08cb5-185">保留</span><span class="sxs-lookup"><span data-stu-id="08cb5-185">reserved</span></span> | <span data-ttu-id="08cb5-186">会议室仅在首次推出时才可用。</span><span class="sxs-lookup"><span data-stu-id="08cb5-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="08cb5-187">无法保留。</span><span class="sxs-lookup"><span data-stu-id="08cb5-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08cb5-188">关系</span><span class="sxs-lookup"><span data-stu-id="08cb5-188">Relationships</span></span>

<span data-ttu-id="08cb5-189">无。</span><span class="sxs-lookup"><span data-stu-id="08cb5-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="08cb5-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08cb5-190">JSON representation</span></span>

<span data-ttu-id="08cb5-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08cb5-191">The following is a JSON representation of the resource.</span></span>

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
