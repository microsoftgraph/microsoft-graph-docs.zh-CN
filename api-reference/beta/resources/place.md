---
title: 放置资源类型
description: 代表一个位置。 这是聊天室或 roomList 的基类型。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ea1736e0215b411673f8c458f79c57181312a25a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521840"
---
# <a name="place-resource-type"></a><span data-ttu-id="1b946-104">放置资源类型</span><span class="sxs-lookup"><span data-stu-id="1b946-104">place resource type</span></span>

<span data-ttu-id="1b946-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1b946-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b946-106">表示基本位置属性，如名称、物理地址和地理坐标。</span><span class="sxs-lookup"><span data-stu-id="1b946-106">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="1b946-107">这是更丰富的位置类型（如[聊天室](room.md)和[roomList](roomlist.md)）的基类型。</span><span class="sxs-lookup"><span data-stu-id="1b946-107">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="1b946-108">使用位置 API</span><span class="sxs-lookup"><span data-stu-id="1b946-108">Using the places API</span></span>
<span data-ttu-id="1b946-109">Exchange Online 管理员可将租户中的会议室组织到会议室列表中。</span><span class="sxs-lookup"><span data-stu-id="1b946-109">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="1b946-110">使用 "位置" API，您可以获取租户中的所有会议室列表或会议室，或获取特定会议室列表中的所有会议室。</span><span class="sxs-lookup"><span data-stu-id="1b946-110">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="1b946-111">位置，如[会议室](room.md)和[roomList](roomlist.md)包含基本**id**、显示名称和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1b946-111">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="1b946-112">此外，它们还包含诸如物理地址和地理坐标等导航信息，在会议室的情况下，其他相关信息（如 AV 功能、楼层号和容量）。</span><span class="sxs-lookup"><span data-stu-id="1b946-112">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="1b946-113">[FindRooms](../api/user-findrooms.md)和[findRoomLists](../api/user-findroomlists.md)函数支持对租户中的会议室和会议室列表进行类似的查找。</span><span class="sxs-lookup"><span data-stu-id="1b946-113">The [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="1b946-114">以下是位置 API 和这些函数之间的比较。</span><span class="sxs-lookup"><span data-stu-id="1b946-114">The following is a comparison between the places API and these functions.</span></span>

|<span data-ttu-id="1b946-115">位置 API</span><span class="sxs-lookup"><span data-stu-id="1b946-115">Places API</span></span> |<span data-ttu-id="1b946-116">findRooms 和 findRoomLists 函数</span><span class="sxs-lookup"><span data-stu-id="1b946-116">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="1b946-117">支持获取租户中的所有会议室或会议室列表，以及会议室列表中的所有会议室</span><span class="sxs-lookup"><span data-stu-id="1b946-117">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="1b946-118">类似的支持-获取租户中的所有会议室或会议室列表，以及会议室列表中的所有会议室</span><span class="sxs-lookup"><span data-stu-id="1b946-118">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="1b946-119">[列表位置](../api/place-list.md)可在租户中返回100个以上的聊天室</span><span class="sxs-lookup"><span data-stu-id="1b946-119">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="1b946-120">[findRooms](../api/user-findrooms.md)返回到租户中的前100个聊天室</span><span class="sxs-lookup"><span data-stu-id="1b946-120">[findRooms](../api/user-findrooms.md) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="1b946-121">支持[获取租户中的单个会议室或会议室列表](../api/place-get.md)</span><span class="sxs-lookup"><span data-stu-id="1b946-121">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="1b946-122">不支持在租户中获取单个会议室或会议室列表</span><span class="sxs-lookup"><span data-stu-id="1b946-122">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="1b946-123">定义[会议室](room.md)和[roomList](roomlist.md)的特定实体，除了显示名称和 SMTP 地址之外，还可指定更丰富的属性集。</span><span class="sxs-lookup"><span data-stu-id="1b946-123">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="1b946-124">每个会议室和会议室列表都是重量较轻的[emailAddress](emailaddress.md)类型，仅指定显示名称和 SMTP 地址</span><span class="sxs-lookup"><span data-stu-id="1b946-124">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="1b946-125">仅支持具有委派（工作或学校帐户）或应用程序权限的组织方案</span><span class="sxs-lookup"><span data-stu-id="1b946-125">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="1b946-126">仅对具有委派或应用程序权限的组织方案的类似支持</span><span class="sxs-lookup"><span data-stu-id="1b946-126">Similar support for only organizational scenarios with delegated or application permissions</span></span>|
|<span data-ttu-id="1b946-127">支持[更新租户中的单个会议室或会议室列表](../api/place-update.md)</span><span class="sxs-lookup"><span data-stu-id="1b946-127">Supports [updating an individual room or room list](../api/place-update.md) in a tenant</span></span> | <span data-ttu-id="1b946-128">不支持更新租户中的单个会议室或会议室列表</span><span class="sxs-lookup"><span data-stu-id="1b946-128">Does not support updating an individual room or room list in a tenant</span></span>

## <a name="methods"></a><span data-ttu-id="1b946-129">方法</span><span class="sxs-lookup"><span data-stu-id="1b946-129">Methods</span></span>

| <span data-ttu-id="1b946-130">方法</span><span class="sxs-lookup"><span data-stu-id="1b946-130">Method</span></span>                              | <span data-ttu-id="1b946-131">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b946-131">Return Type</span></span>                  | <span data-ttu-id="1b946-132">说明</span><span class="sxs-lookup"><span data-stu-id="1b946-132">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="1b946-133">列表位置</span><span class="sxs-lookup"><span data-stu-id="1b946-133">List places</span></span>](../api/place-list.md) | <span data-ttu-id="1b946-134">所请求的派生类型的[位置](place.md)的集合</span><span class="sxs-lookup"><span data-stu-id="1b946-134">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="1b946-135">获取在租户中定义的指定类型的**位置**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1b946-135">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="1b946-136">获取位置</span><span class="sxs-lookup"><span data-stu-id="1b946-136">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="1b946-137">所请求的派生类型的[位置](place.md)</span><span class="sxs-lookup"><span data-stu-id="1b946-137">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="1b946-138">获取指定的**place**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b946-138">Get the properties and relationships of a specified **place** object.</span></span> |
| [<span data-ttu-id="1b946-139">更新位置</span><span class="sxs-lookup"><span data-stu-id="1b946-139">Update place</span></span>](../api/place-update.md)    | <span data-ttu-id="1b946-140">所请求的派生类型的[位置](place.md)</span><span class="sxs-lookup"><span data-stu-id="1b946-140">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="1b946-141">更新指定的**place**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b946-141">Update the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b946-142">属性</span><span class="sxs-lookup"><span data-stu-id="1b946-142">Properties</span></span>

| <span data-ttu-id="1b946-143">属性</span><span class="sxs-lookup"><span data-stu-id="1b946-143">Property</span></span>       | <span data-ttu-id="1b946-144">类型</span><span class="sxs-lookup"><span data-stu-id="1b946-144">Type</span></span>                                              | <span data-ttu-id="1b946-145">说明</span><span class="sxs-lookup"><span data-stu-id="1b946-145">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="1b946-146">address</span><span class="sxs-lookup"><span data-stu-id="1b946-146">address</span></span>        | [<span data-ttu-id="1b946-147">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="1b946-147">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="1b946-148">地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="1b946-148">The street address of the place.</span></span> |
| <span data-ttu-id="1b946-149">displayName</span><span class="sxs-lookup"><span data-stu-id="1b946-149">displayName</span></span>    | <span data-ttu-id="1b946-150">字符串</span><span class="sxs-lookup"><span data-stu-id="1b946-150">String</span></span>                                            | <span data-ttu-id="1b946-151">与位置关联的名称。</span><span class="sxs-lookup"><span data-stu-id="1b946-151">The name associated with the place.</span></span> |
| <span data-ttu-id="1b946-152">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="1b946-152">geoCoordinates</span></span> | [<span data-ttu-id="1b946-153">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="1b946-153">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="1b946-154">指定纬度、经度和（可选）海拔高度坐标中的位置。</span><span class="sxs-lookup"><span data-stu-id="1b946-154">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="1b946-155">id</span><span class="sxs-lookup"><span data-stu-id="1b946-155">id</span></span>             | <span data-ttu-id="1b946-156">String</span><span class="sxs-lookup"><span data-stu-id="1b946-156">String</span></span>                                            | <span data-ttu-id="1b946-157">位置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1b946-157">Unique identifier for the place.</span></span> <span data-ttu-id="1b946-158">只读。</span><span class="sxs-lookup"><span data-stu-id="1b946-158">Read-only.</span></span> |
| <span data-ttu-id="1b946-159">phone</span><span class="sxs-lookup"><span data-stu-id="1b946-159">phone</span></span>          | <span data-ttu-id="1b946-160">String</span><span class="sxs-lookup"><span data-stu-id="1b946-160">String</span></span>                                            | <span data-ttu-id="1b946-161">地点的电话号码。</span><span class="sxs-lookup"><span data-stu-id="1b946-161">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1b946-162">关系</span><span class="sxs-lookup"><span data-stu-id="1b946-162">Relationships</span></span>

<span data-ttu-id="1b946-163">无。</span><span class="sxs-lookup"><span data-stu-id="1b946-163">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b946-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b946-164">JSON representation</span></span>

<span data-ttu-id="1b946-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b946-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place",
  "baseType": ""
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

## <a name="see-also"></a><span data-ttu-id="1b946-166">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1b946-166">See also</span></span>
- <span data-ttu-id="1b946-167">若要使管理员能够创建会议室列表，请使用 Exchange PowerShell cmdlet [new-distributiongroup](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="1b946-167">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="1b946-168">若要使管理员向会议室列表中添加聊天室，请使用 Exchange Powershell cmdlet[外接程序 get-distributiongroupmember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="1b946-168">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
