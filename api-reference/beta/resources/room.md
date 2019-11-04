---
title: 会议室资源类型
description: 指定租户中聊天室的属性。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: cfa1d87093c7f843dd9a8294a253751726b3d34b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938721"
---
# <a name="room-resource-type"></a><span data-ttu-id="14df3-103">会议室资源类型</span><span class="sxs-lookup"><span data-stu-id="14df3-103">room resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14df3-104">表示租户中的会议室。</span><span class="sxs-lookup"><span data-stu-id="14df3-104">Represents a room in a tenant.</span></span> 

<span data-ttu-id="14df3-105">在 Exchange Online 中，每个会议室都与一个会议室邮箱相关联。</span><span class="sxs-lookup"><span data-stu-id="14df3-105">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="14df3-106">从[原位置](place.md)派生。</span><span class="sxs-lookup"><span data-stu-id="14df3-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="14df3-107">方法</span><span class="sxs-lookup"><span data-stu-id="14df3-107">Methods</span></span>

| <span data-ttu-id="14df3-108">方法</span><span class="sxs-lookup"><span data-stu-id="14df3-108">Method</span></span>                              | <span data-ttu-id="14df3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="14df3-109">Return Type</span></span>                  | <span data-ttu-id="14df3-110">说明</span><span class="sxs-lookup"><span data-stu-id="14df3-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="14df3-111">列表位置</span><span class="sxs-lookup"><span data-stu-id="14df3-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="14df3-112">所请求的派生类型的[位置](place.md)的集合</span><span class="sxs-lookup"><span data-stu-id="14df3-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="14df3-113">获取在租户中定义的指定类型的**位置**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="14df3-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="14df3-114">例如，您可以获取租户中的所有会议室、所有会议室列表或特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="14df3-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="14df3-115">获取位置</span><span class="sxs-lookup"><span data-stu-id="14df3-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="14df3-116">所请求的派生类型的[位置](place.md)</span><span class="sxs-lookup"><span data-stu-id="14df3-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="14df3-117">获取指定的**place**对象（例如会议室）的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14df3-117">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="14df3-118">属性</span><span class="sxs-lookup"><span data-stu-id="14df3-118">Properties</span></span>

| <span data-ttu-id="14df3-119">属性</span><span class="sxs-lookup"><span data-stu-id="14df3-119">Property</span></span>               | <span data-ttu-id="14df3-120">类型</span><span class="sxs-lookup"><span data-stu-id="14df3-120">Type</span></span>                                              | <span data-ttu-id="14df3-121">描述</span><span class="sxs-lookup"><span data-stu-id="14df3-121">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="14df3-122">address</span><span class="sxs-lookup"><span data-stu-id="14df3-122">address</span></span>                | [<span data-ttu-id="14df3-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="14df3-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="14df3-124">会议室的街道地址。</span><span class="sxs-lookup"><span data-stu-id="14df3-124">The street address of the room.</span></span> |
| <span data-ttu-id="14df3-125">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="14df3-125">audioDeviceName</span></span>        | <span data-ttu-id="14df3-126">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-126">String</span></span>                                            | <span data-ttu-id="14df3-127">指定会议室中音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="14df3-127">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="14df3-128">bookingType</span><span class="sxs-lookup"><span data-stu-id="14df3-128">bookingType</span></span>            | [<span data-ttu-id="14df3-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="14df3-129">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="14df3-130">会议室的类型。</span><span class="sxs-lookup"><span data-stu-id="14df3-130">Type of room.</span></span> <span data-ttu-id="14df3-131">可能的值`standard`为和`reserved`。</span><span class="sxs-lookup"><span data-stu-id="14df3-131">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="14df3-132">幢</span><span class="sxs-lookup"><span data-stu-id="14df3-132">building</span></span>               | <span data-ttu-id="14df3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-133">String</span></span>                                            | <span data-ttu-id="14df3-134">指定聊天室所在的建筑物名称或楼号。</span><span class="sxs-lookup"><span data-stu-id="14df3-134">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="14df3-135">能够</span><span class="sxs-lookup"><span data-stu-id="14df3-135">capacity</span></span>               | <span data-ttu-id="14df3-136">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-136">String</span></span>                                            | <span data-ttu-id="14df3-137">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="14df3-137">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="14df3-138">displayName</span><span class="sxs-lookup"><span data-stu-id="14df3-138">displayName</span></span>            | <span data-ttu-id="14df3-139">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-139">String</span></span>                                            | <span data-ttu-id="14df3-140">与聊天室关联的名称。</span><span class="sxs-lookup"><span data-stu-id="14df3-140">The name associated with the room.</span></span> |
| <span data-ttu-id="14df3-141">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="14df3-141">displayDeviceName</span></span>      | <span data-ttu-id="14df3-142">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-142">String</span></span>                                            | <span data-ttu-id="14df3-143">指定聊天室中显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="14df3-143">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="14df3-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="14df3-144">emailAddress</span></span>           | <span data-ttu-id="14df3-145">String</span><span class="sxs-lookup"><span data-stu-id="14df3-145">String</span></span>                                            | <span data-ttu-id="14df3-146">聊天室的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="14df3-146">Email address of the room.</span></span> |
| <span data-ttu-id="14df3-147">floorLabel</span><span class="sxs-lookup"><span data-stu-id="14df3-147">floorLabel</span></span>             | <span data-ttu-id="14df3-148">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-148">String</span></span>                                            | <span data-ttu-id="14df3-149">指定基底的描述性标签，例如 P。</span><span class="sxs-lookup"><span data-stu-id="14df3-149">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="14df3-150">floorNumber</span><span class="sxs-lookup"><span data-stu-id="14df3-150">floorNumber</span></span>            | <span data-ttu-id="14df3-151">Int32</span><span class="sxs-lookup"><span data-stu-id="14df3-151">Int32</span></span>                                             | <span data-ttu-id="14df3-152">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="14df3-152">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="14df3-153">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="14df3-153">geoCoordinates</span></span>         | [<span data-ttu-id="14df3-154">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="14df3-154">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="14df3-155">指定纬度、经度和（可选）海拔坐标中的会议室位置。</span><span class="sxs-lookup"><span data-stu-id="14df3-155">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="14df3-156">id</span><span class="sxs-lookup"><span data-stu-id="14df3-156">id</span></span>                     | <span data-ttu-id="14df3-157">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-157">String</span></span>                                            | <span data-ttu-id="14df3-158">聊天室的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="14df3-158">Unique identifier for the room.</span></span> <span data-ttu-id="14df3-159">只读。</span><span class="sxs-lookup"><span data-stu-id="14df3-159">Read-only.</span></span> |
| <span data-ttu-id="14df3-160">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="14df3-160">isWheelchairAccessible</span></span> | <span data-ttu-id="14df3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="14df3-161">Boolean</span></span>                                           | <span data-ttu-id="14df3-162">指定会议室是否 wheelchair 可访问。</span><span class="sxs-lookup"><span data-stu-id="14df3-162">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="14df3-163">label</span><span class="sxs-lookup"><span data-stu-id="14df3-163">label</span></span>                  | <span data-ttu-id="14df3-164">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-164">String</span></span>                                            | <span data-ttu-id="14df3-165">指定聊天室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="14df3-165">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="14df3-166">昵称</span><span class="sxs-lookup"><span data-stu-id="14df3-166">nickname</span></span>               | <span data-ttu-id="14df3-167">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-167">String</span></span>                                            | <span data-ttu-id="14df3-168">指定聊天室的昵称，例如 "会议室"。</span><span class="sxs-lookup"><span data-stu-id="14df3-168">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="14df3-169">phone</span><span class="sxs-lookup"><span data-stu-id="14df3-169">phone</span></span>                  | <span data-ttu-id="14df3-170">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-170">String</span></span>                                            | <span data-ttu-id="14df3-171">会议室的电话号码。</span><span class="sxs-lookup"><span data-stu-id="14df3-171">The phone number of the room.</span></span> |
| <span data-ttu-id="14df3-172">标记</span><span class="sxs-lookup"><span data-stu-id="14df3-172">tags</span></span>                   | <span data-ttu-id="14df3-173">String collection</span><span class="sxs-lookup"><span data-stu-id="14df3-173">String collection</span></span>                                 | <span data-ttu-id="14df3-174">指定会议室的其他功能，例如，视图类型或家具类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="14df3-174">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="14df3-175">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="14df3-175">videoDeviceName</span></span>        | <span data-ttu-id="14df3-176">字符串</span><span class="sxs-lookup"><span data-stu-id="14df3-176">String</span></span>                                            | <span data-ttu-id="14df3-177">指定聊天室中视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="14df3-177">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="14df3-178">bookingType 值</span><span class="sxs-lookup"><span data-stu-id="14df3-178">bookingType values</span></span>

| <span data-ttu-id="14df3-179">值</span><span class="sxs-lookup"><span data-stu-id="14df3-179">Value</span></span>    | <span data-ttu-id="14df3-180">说明</span><span class="sxs-lookup"><span data-stu-id="14df3-180">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="14df3-181">普通</span><span class="sxs-lookup"><span data-stu-id="14df3-181">standard</span></span> | <span data-ttu-id="14df3-182">可以根据此 cmdlet 中的其他设置保留该会议室。</span><span class="sxs-lookup"><span data-stu-id="14df3-182">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="14df3-183">所有者、作者和网站所有者仍可以访问此项目。</span><span class="sxs-lookup"><span data-stu-id="14df3-183">This is the default value.</span></span> |
| <span data-ttu-id="14df3-184">保留</span><span class="sxs-lookup"><span data-stu-id="14df3-184">reserved</span></span> | <span data-ttu-id="14df3-185">会议室仅在首次推出时才可用。</span><span class="sxs-lookup"><span data-stu-id="14df3-185">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="14df3-186">无法保留。</span><span class="sxs-lookup"><span data-stu-id="14df3-186">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14df3-187">关系</span><span class="sxs-lookup"><span data-stu-id="14df3-187">Relationships</span></span>

<span data-ttu-id="14df3-188">无。</span><span class="sxs-lookup"><span data-stu-id="14df3-188">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14df3-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14df3-189">JSON representation</span></span>

<span data-ttu-id="14df3-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14df3-190">The following is a JSON representation of the resource.</span></span>

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
