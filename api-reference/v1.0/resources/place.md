---
title: place 资源类型
description: 表示位置。 这是会议室或 roomList 的基本类型。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0897cf9105ae0260803fa81291ab879bd7876b86
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156341"
---
# <a name="place-resource-type"></a><span data-ttu-id="879f5-104">place 资源类型</span><span class="sxs-lookup"><span data-stu-id="879f5-104">place resource type</span></span>

<span data-ttu-id="879f5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="879f5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="879f5-106">表示基本的位置属性，如名称、物理地址和地理坐标。</span><span class="sxs-lookup"><span data-stu-id="879f5-106">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="879f5-107">这是更丰富的位置类型（如 room 和[](room.md) [roomList）的基本类型](roomlist.md)。</span><span class="sxs-lookup"><span data-stu-id="879f5-107">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="879f5-108">使用位置 API</span><span class="sxs-lookup"><span data-stu-id="879f5-108">Using the places API</span></span>
<span data-ttu-id="879f5-109">Exchange Online 管理员可以将租户中的会议室组织到会议室列表中。</span><span class="sxs-lookup"><span data-stu-id="879f5-109">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="879f5-110">使用位置 API，可以获取租户中所有会议室列表或会议室，或获取特定会议室列表中的所有会议室。</span><span class="sxs-lookup"><span data-stu-id="879f5-110">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="879f5-111">会议室 [和 roomList](room.md)等位置包含基本 [](roomlist.md)**id、显示名称** 和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="879f5-111">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="879f5-112">此外，它们包含导航信息（如物理地址和地理坐标）以及房间信息、其他相关信息（如 AV 功能、楼层和容量）。</span><span class="sxs-lookup"><span data-stu-id="879f5-112">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="879f5-113">[findRooms 和](/graph/api/user-findrooms) [findRoomLists](/graph/api/user-findroomlists)函数支持对租户中的会议室和会议室列表进行类似的查找。</span><span class="sxs-lookup"><span data-stu-id="879f5-113">The [findRooms](/graph/api/user-findrooms) and [findRoomLists](/graph/api/user-findroomlists) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="879f5-114">下面是位置 API 和这些函数之间的比较。</span><span class="sxs-lookup"><span data-stu-id="879f5-114">The following is a comparison between the places API and these functions.</span></span>  <span data-ttu-id="879f5-115">如果要创建生产应用，请选择位置 API，因为 API 现已在 v1.0 中普遍提供。</span><span class="sxs-lookup"><span data-stu-id="879f5-115">If you are creating a production app, choose the places API as the API is now generally available in v1.0.</span></span> <span data-ttu-id="879f5-116">计划更新使用 **findRooms** 或 **findRoomLists** 使用位置 API 的任何现有代码，因为 **findRooms** 或 **findRoomLists** 将弃用，并且将公布时间线。</span><span class="sxs-lookup"><span data-stu-id="879f5-116">Plan to update any existing code that uses **findRooms** or **findRoomLists** to use the places API, because **findRooms** or **findRoomLists** will be deprecated, and a timeline will be announced.</span></span>

|<span data-ttu-id="879f5-117">Places API</span><span class="sxs-lookup"><span data-stu-id="879f5-117">Places API</span></span> |<span data-ttu-id="879f5-118">findRooms 和 findRoomLists 函数</span><span class="sxs-lookup"><span data-stu-id="879f5-118">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="879f5-119">支持获取租户中所有会议室或会议室列表，以及会议室列表中的所有会议室</span><span class="sxs-lookup"><span data-stu-id="879f5-119">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="879f5-120">类似支持 - 获取租户中所有会议室或会议室列表，以及会议室列表中的所有会议室</span><span class="sxs-lookup"><span data-stu-id="879f5-120">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="879f5-121">[列出位置](../api/place-list.md) 可以返回租户中的 100 多个会议室</span><span class="sxs-lookup"><span data-stu-id="879f5-121">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="879f5-122">[findRooms](/graph/api/user-findrooms) 最多返回租户中的前 100 个会议室</span><span class="sxs-lookup"><span data-stu-id="879f5-122">[findRooms](/graph/api/user-findrooms) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="879f5-123">支持 [获取租户中的单个会议室](../api/place-get.md) 或会议室列表</span><span class="sxs-lookup"><span data-stu-id="879f5-123">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="879f5-124">不支持获取租户中的单个会议室或会议室列表</span><span class="sxs-lookup"><span data-stu-id="879f5-124">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="879f5-125">定义会议室和[roomList](roomlist.md) [](room.md)的特定实体，这些实体指定更丰富的属性集，以及显示名称 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="879f5-125">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="879f5-126">每个会议室和会议室列表都是一种轻型 [电子邮件](emailaddress.md) 地址类型，它仅指定显示名称 SMTP 地址</span><span class="sxs-lookup"><span data-stu-id="879f5-126">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="879f5-127">仅支持具有委派工作 (学校帐户或) 或应用程序权限的组织方案</span><span class="sxs-lookup"><span data-stu-id="879f5-127">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="879f5-128">仅对具有委派权限或应用程序权限的组织方案的类似支持</span><span class="sxs-lookup"><span data-stu-id="879f5-128">Similar support for only organizational scenarios with delegated or application permissions</span></span>|
|<span data-ttu-id="879f5-129">支持 [更新租户中的单个会议室](../api/place-update.md) 或会议室列表</span><span class="sxs-lookup"><span data-stu-id="879f5-129">Supports [updating an individual room or room list](../api/place-update.md) in a tenant</span></span> | <span data-ttu-id="879f5-130">不支持更新租户中的单个会议室或会议室列表</span><span class="sxs-lookup"><span data-stu-id="879f5-130">Does not support updating an individual room or room list in a tenant</span></span>

## <a name="methods"></a><span data-ttu-id="879f5-131">方法</span><span class="sxs-lookup"><span data-stu-id="879f5-131">Methods</span></span>

| <span data-ttu-id="879f5-132">方法</span><span class="sxs-lookup"><span data-stu-id="879f5-132">Method</span></span>                              | <span data-ttu-id="879f5-133">返回类型</span><span class="sxs-lookup"><span data-stu-id="879f5-133">Return Type</span></span>                  | <span data-ttu-id="879f5-134">说明</span><span class="sxs-lookup"><span data-stu-id="879f5-134">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="879f5-135">列出位置</span><span class="sxs-lookup"><span data-stu-id="879f5-135">List places</span></span>](../api/place-list.md) | <span data-ttu-id="879f5-136">所请求的派生位置类型 [的集合](place.md)</span><span class="sxs-lookup"><span data-stu-id="879f5-136">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="879f5-137">获取租户中定义的指定类型的 **place** 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="879f5-137">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="879f5-138">获取位置</span><span class="sxs-lookup"><span data-stu-id="879f5-138">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="879f5-139">请求的派生位置 [类型](place.md)</span><span class="sxs-lookup"><span data-stu-id="879f5-139">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="879f5-140">获取指定 place 对象 **的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="879f5-140">Get the properties and relationships of a specified **place** object.</span></span> |
| [<span data-ttu-id="879f5-141">更新位置</span><span class="sxs-lookup"><span data-stu-id="879f5-141">Update place</span></span>](../api/place-update.md)    | <span data-ttu-id="879f5-142">请求的派生位置 [类型](place.md)</span><span class="sxs-lookup"><span data-stu-id="879f5-142">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="879f5-143">更新指定 place 对象 **的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="879f5-143">Update the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="879f5-144">属性</span><span class="sxs-lookup"><span data-stu-id="879f5-144">Properties</span></span>

| <span data-ttu-id="879f5-145">属性</span><span class="sxs-lookup"><span data-stu-id="879f5-145">Property</span></span>       | <span data-ttu-id="879f5-146">类型</span><span class="sxs-lookup"><span data-stu-id="879f5-146">Type</span></span>                                              | <span data-ttu-id="879f5-147">说明</span><span class="sxs-lookup"><span data-stu-id="879f5-147">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="879f5-148">address</span><span class="sxs-lookup"><span data-stu-id="879f5-148">address</span></span>        | [<span data-ttu-id="879f5-149">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="879f5-149">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="879f5-150">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="879f5-150">The street address of the place.</span></span> |
| <span data-ttu-id="879f5-151">displayName</span><span class="sxs-lookup"><span data-stu-id="879f5-151">displayName</span></span>    | <span data-ttu-id="879f5-152">String</span><span class="sxs-lookup"><span data-stu-id="879f5-152">String</span></span>                                            | <span data-ttu-id="879f5-153">与位置关联的名称。</span><span class="sxs-lookup"><span data-stu-id="879f5-153">The name associated with the place.</span></span> |
| <span data-ttu-id="879f5-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="879f5-154">geoCoordinates</span></span> | [<span data-ttu-id="879f5-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="879f5-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="879f5-156">指定以纬度、经度和纬度（可选） (高度坐标) 位置。</span><span class="sxs-lookup"><span data-stu-id="879f5-156">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="879f5-157">id</span><span class="sxs-lookup"><span data-stu-id="879f5-157">id</span></span>             | <span data-ttu-id="879f5-158">String</span><span class="sxs-lookup"><span data-stu-id="879f5-158">String</span></span>                                            | <span data-ttu-id="879f5-159">位置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="879f5-159">Unique identifier for the place.</span></span> <span data-ttu-id="879f5-160">只读。</span><span class="sxs-lookup"><span data-stu-id="879f5-160">Read-only.</span></span> |
| <span data-ttu-id="879f5-161">phone</span><span class="sxs-lookup"><span data-stu-id="879f5-161">phone</span></span>          | <span data-ttu-id="879f5-162">String</span><span class="sxs-lookup"><span data-stu-id="879f5-162">String</span></span>                                            | <span data-ttu-id="879f5-163">位置的电话号码。</span><span class="sxs-lookup"><span data-stu-id="879f5-163">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="879f5-164">关系</span><span class="sxs-lookup"><span data-stu-id="879f5-164">Relationships</span></span>

<span data-ttu-id="879f5-165">无。</span><span class="sxs-lookup"><span data-stu-id="879f5-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="879f5-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="879f5-166">JSON representation</span></span>

<span data-ttu-id="879f5-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="879f5-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "id": "String (identifier)",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "phone": "String"
}
```

## <a name="see-also"></a><span data-ttu-id="879f5-168">另请参阅</span><span class="sxs-lookup"><span data-stu-id="879f5-168">See also</span></span>
- <span data-ttu-id="879f5-169">若要使管理员创建会议室列表，请使用 Exchange PowerShell cmdlet [New-DistributionGroup。](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="879f5-169">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="879f5-170">对于将会议室添加到会议室列表的管理员，请使用 Exchange Powershell cmdlet [Add-DistributionGroupMember。](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="879f5-170">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
