---
title: bookingService 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c6cf62320a6cfd8e96455e95e1d17c0621d261f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328308"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="987e0-104">bookingService 资源类型</span><span class="sxs-lookup"><span data-stu-id="987e0-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="987e0-105">表示有关[bookingBusiness](bookingbusiness.md)提供的特定服务的信息, 如服务名称、价格和通常提供此类服务的人员。</span><span class="sxs-lookup"><span data-stu-id="987e0-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="987e0-106">方法</span><span class="sxs-lookup"><span data-stu-id="987e0-106">Methods</span></span>

| <span data-ttu-id="987e0-107">方法</span><span class="sxs-lookup"><span data-stu-id="987e0-107">Method</span></span>           | <span data-ttu-id="987e0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="987e0-108">Return Type</span></span>    |<span data-ttu-id="987e0-109">说明</span><span class="sxs-lookup"><span data-stu-id="987e0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="987e0-110">列出服务</span><span class="sxs-lookup"><span data-stu-id="987e0-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="987e0-111">[bookingService](bookingservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="987e0-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="987e0-112">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="987e0-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="987e0-113">创建 bookingService</span><span class="sxs-lookup"><span data-stu-id="987e0-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="987e0-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="987e0-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="987e0-115">为指定的[bookingbusiness](../resources/bookingbusiness.md)创建**bookingService** 。</span><span class="sxs-lookup"><span data-stu-id="987e0-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="987e0-116">获取 bookingService</span><span class="sxs-lookup"><span data-stu-id="987e0-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="987e0-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="987e0-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="987e0-118">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="987e0-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="987e0-119">更新</span><span class="sxs-lookup"><span data-stu-id="987e0-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="987e0-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="987e0-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="987e0-121">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象。</span><span class="sxs-lookup"><span data-stu-id="987e0-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="987e0-122">删除</span><span class="sxs-lookup"><span data-stu-id="987e0-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="987e0-123">无</span><span class="sxs-lookup"><span data-stu-id="987e0-123">None</span></span> |<span data-ttu-id="987e0-124">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象。</span><span class="sxs-lookup"><span data-stu-id="987e0-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="987e0-125">属性</span><span class="sxs-lookup"><span data-stu-id="987e0-125">Properties</span></span>
| <span data-ttu-id="987e0-126">属性</span><span class="sxs-lookup"><span data-stu-id="987e0-126">Property</span></span>     | <span data-ttu-id="987e0-127">类型</span><span class="sxs-lookup"><span data-stu-id="987e0-127">Type</span></span>   |<span data-ttu-id="987e0-128">说明</span><span class="sxs-lookup"><span data-stu-id="987e0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="987e0-129">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="987e0-129">defaultDuration</span></span>|<span data-ttu-id="987e0-130">持续时间</span><span class="sxs-lookup"><span data-stu-id="987e0-130">Duration</span></span>|<span data-ttu-id="987e0-131">服务的默认长度, 以天数、小时数、分钟数和秒数表示。</span><span class="sxs-lookup"><span data-stu-id="987e0-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="987e0-132">例如, p11d23h59m 59.999999999999 s。</span><span class="sxs-lookup"><span data-stu-id="987e0-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="987e0-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="987e0-133">defaultLocation</span></span>|[<span data-ttu-id="987e0-134">location</span><span class="sxs-lookup"><span data-stu-id="987e0-134">location</span></span>](location.md)|<span data-ttu-id="987e0-135">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="987e0-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="987e0-136">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="987e0-136">defaultPrice</span></span>|<span data-ttu-id="987e0-137">双精度</span><span class="sxs-lookup"><span data-stu-id="987e0-137">Double</span></span>|<span data-ttu-id="987e0-138">服务的默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="987e0-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="987e0-139">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="987e0-139">defaultPriceType</span></span>|<span data-ttu-id="987e0-140">string</span><span class="sxs-lookup"><span data-stu-id="987e0-140">string</span></span>|<span data-ttu-id="987e0-141">服务收费的默认方式。</span><span class="sxs-lookup"><span data-stu-id="987e0-141">The default way the service is charged.</span></span> <span data-ttu-id="987e0-142">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="987e0-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="987e0-143">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="987e0-143">defaultReminders</span></span>|<span data-ttu-id="987e0-144">[bookingReminder](bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="987e0-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="987e0-145">此服务的约会的默认提醒集。</span><span class="sxs-lookup"><span data-stu-id="987e0-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="987e0-146">此属性的值仅在按 ID 读取此**bookingService**时可用。</span><span class="sxs-lookup"><span data-stu-id="987e0-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="987e0-147">说明</span><span class="sxs-lookup"><span data-stu-id="987e0-147">description</span></span>|<span data-ttu-id="987e0-148">String</span><span class="sxs-lookup"><span data-stu-id="987e0-148">String</span></span>|<span data-ttu-id="987e0-149">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="987e0-149">A text description for the service.</span></span>|
|<span data-ttu-id="987e0-150">displayName</span><span class="sxs-lookup"><span data-stu-id="987e0-150">displayName</span></span>|<span data-ttu-id="987e0-151">字符串</span><span class="sxs-lookup"><span data-stu-id="987e0-151">String</span></span>|<span data-ttu-id="987e0-152">服务名称。</span><span class="sxs-lookup"><span data-stu-id="987e0-152">A service name.</span></span>|
|<span data-ttu-id="987e0-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="987e0-153">emailAddress</span></span>|<span data-ttu-id="987e0-154">String</span><span class="sxs-lookup"><span data-stu-id="987e0-154">String</span></span>|<span data-ttu-id="987e0-155">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="987e0-155">An email address</span></span>|
|<span data-ttu-id="987e0-156">id</span><span class="sxs-lookup"><span data-stu-id="987e0-156">id</span></span>|<span data-ttu-id="987e0-157">字符串</span><span class="sxs-lookup"><span data-stu-id="987e0-157">String</span></span>|<span data-ttu-id="987e0-158">该服务的 ID (采用 GUID 格式)。</span><span class="sxs-lookup"><span data-stu-id="987e0-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="987e0-159">只读。</span><span class="sxs-lookup"><span data-stu-id="987e0-159">Read-only.</span></span>|
|<span data-ttu-id="987e0-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="987e0-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="987e0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="987e0-161">Boolean</span></span>|<span data-ttu-id="987e0-162">如果为 True, 则表示此服务不可供客户预订。</span><span class="sxs-lookup"><span data-stu-id="987e0-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="987e0-163">notes</span><span class="sxs-lookup"><span data-stu-id="987e0-163">notes</span></span>|<span data-ttu-id="987e0-164">String</span><span class="sxs-lookup"><span data-stu-id="987e0-164">String</span></span>|<span data-ttu-id="987e0-165">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="987e0-165">Additional information about this service.</span></span>|
|<span data-ttu-id="987e0-166">postBuffer</span><span class="sxs-lookup"><span data-stu-id="987e0-166">postBuffer</span></span>|<span data-ttu-id="987e0-167">持续时间</span><span class="sxs-lookup"><span data-stu-id="987e0-167">Duration</span></span>|<span data-ttu-id="987e0-168">此服务的约会结束后以及下一个客户约会可以被预订前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="987e0-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="987e0-169">preBuffer</span><span class="sxs-lookup"><span data-stu-id="987e0-169">preBuffer</span></span>|<span data-ttu-id="987e0-170">持续时间</span><span class="sxs-lookup"><span data-stu-id="987e0-170">Duration</span></span>|<span data-ttu-id="987e0-171">在此服务的约会开始之前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="987e0-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="987e0-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="987e0-172">schedulingPolicy</span></span>|[<span data-ttu-id="987e0-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="987e0-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="987e0-174">确定应如何创建和管理此类服务的约会的一组策略。</span><span class="sxs-lookup"><span data-stu-id="987e0-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="987e0-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="987e0-175">staffMemberIds</span></span>|<span data-ttu-id="987e0-176">String 集合</span><span class="sxs-lookup"><span data-stu-id="987e0-176">String collection</span></span>|<span data-ttu-id="987e0-177">代表提供此服务的[教职员工成员](bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="987e0-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="987e0-178">关系</span><span class="sxs-lookup"><span data-stu-id="987e0-178">Relationships</span></span>
<span data-ttu-id="987e0-179">无</span><span class="sxs-lookup"><span data-stu-id="987e0-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="987e0-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="987e0-180">JSON representation</span></span>

<span data-ttu-id="987e0-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="987e0-181">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
