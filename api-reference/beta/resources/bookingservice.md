---
title: bookingService 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 63eae84249501426c43ad73326cbf005009753be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815440"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="a2f6a-104">bookingService 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2f6a-104">bookingService resource type</span></span>

 > <span data-ttu-id="a2f6a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2f6a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="a2f6a-107">代表由[bookingBusiness](bookingbusiness.md)，如的服务名称、 价格和通常提供了此类服务的人员提供的特定服务的信息。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-107">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="a2f6a-108">方法</span><span class="sxs-lookup"><span data-stu-id="a2f6a-108">Methods</span></span>

| <span data-ttu-id="a2f6a-109">方法</span><span class="sxs-lookup"><span data-stu-id="a2f6a-109">Method</span></span>           | <span data-ttu-id="a2f6a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2f6a-110">Return Type</span></span>    |<span data-ttu-id="a2f6a-111">说明</span><span class="sxs-lookup"><span data-stu-id="a2f6a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2f6a-112">列表服务</span><span class="sxs-lookup"><span data-stu-id="a2f6a-112">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="a2f6a-113">[bookingService](bookingservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2f6a-113">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="a2f6a-114">指定[bookingbusiness](../resources/bookingbusiness.md)中获取**bookingService**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-114">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="a2f6a-115">创建 bookingService</span><span class="sxs-lookup"><span data-stu-id="a2f6a-115">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="a2f6a-116">bookingService</span><span class="sxs-lookup"><span data-stu-id="a2f6a-116">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="a2f6a-117">创建用于指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService** 。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-117">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="a2f6a-118">获取 bookingService</span><span class="sxs-lookup"><span data-stu-id="a2f6a-118">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="a2f6a-119">bookingService</span><span class="sxs-lookup"><span data-stu-id="a2f6a-119">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="a2f6a-120">指定[bookingbusiness](../resources/bookingbusiness.md)中获取的属性和**bookingService**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-120">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="a2f6a-121">Update</span><span class="sxs-lookup"><span data-stu-id="a2f6a-121">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="a2f6a-122">bookingService</span><span class="sxs-lookup"><span data-stu-id="a2f6a-122">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="a2f6a-123">更新中指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService**对象。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-123">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="a2f6a-124">删除</span><span class="sxs-lookup"><span data-stu-id="a2f6a-124">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="a2f6a-125">无</span><span class="sxs-lookup"><span data-stu-id="a2f6a-125">None</span></span> |<span data-ttu-id="a2f6a-126">删除在指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService**对象。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-126">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="a2f6a-127">属性</span><span class="sxs-lookup"><span data-stu-id="a2f6a-127">Properties</span></span>
| <span data-ttu-id="a2f6a-128">属性</span><span class="sxs-lookup"><span data-stu-id="a2f6a-128">Property</span></span>     | <span data-ttu-id="a2f6a-129">类型</span><span class="sxs-lookup"><span data-stu-id="a2f6a-129">Type</span></span>   |<span data-ttu-id="a2f6a-130">Description</span><span class="sxs-lookup"><span data-stu-id="a2f6a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2f6a-131">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="a2f6a-131">defaultDuration</span></span>|<span data-ttu-id="a2f6a-132">Duration</span><span class="sxs-lookup"><span data-stu-id="a2f6a-132">Duration</span></span>|<span data-ttu-id="a2f6a-133">默认服务中的天、 小时、 分钟和秒数字表示的长度。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-133">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="a2f6a-134">例如，P11D23H59M59.999999999999S。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-134">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="a2f6a-135">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="a2f6a-135">defaultLocation</span></span>|[<span data-ttu-id="a2f6a-136">location</span><span class="sxs-lookup"><span data-stu-id="a2f6a-136">location</span></span>](location.md)|<span data-ttu-id="a2f6a-137">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-137">The default physical location for the service.</span></span>|
|<span data-ttu-id="a2f6a-138">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="a2f6a-138">defaultPrice</span></span>|<span data-ttu-id="a2f6a-139">Double</span><span class="sxs-lookup"><span data-stu-id="a2f6a-139">Double</span></span>|<span data-ttu-id="a2f6a-140">该服务默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-140">The default monetary price for the service.</span></span>|
|<span data-ttu-id="a2f6a-141">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="a2f6a-141">defaultPriceType</span></span>|<span data-ttu-id="a2f6a-142">string</span><span class="sxs-lookup"><span data-stu-id="a2f6a-142">string</span></span>|<span data-ttu-id="a2f6a-143">负责服务的默认方式。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-143">The default way the service is charged.</span></span> <span data-ttu-id="a2f6a-144">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-144">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="a2f6a-145">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="a2f6a-145">defaultReminders</span></span>|<span data-ttu-id="a2f6a-146">[bookingReminder](bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2f6a-146">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="a2f6a-147">默认设置的该服务的约会的提醒。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-147">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="a2f6a-148">此属性的值时，可仅读取此**bookingService**由其 id。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-148">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="a2f6a-149">说明</span><span class="sxs-lookup"><span data-stu-id="a2f6a-149">description</span></span>|<span data-ttu-id="a2f6a-150">字符串</span><span class="sxs-lookup"><span data-stu-id="a2f6a-150">String</span></span>|<span data-ttu-id="a2f6a-151">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-151">A text description for the service.</span></span>|
|<span data-ttu-id="a2f6a-152">displayName</span><span class="sxs-lookup"><span data-stu-id="a2f6a-152">displayName</span></span>|<span data-ttu-id="a2f6a-153">字符串</span><span class="sxs-lookup"><span data-stu-id="a2f6a-153">String</span></span>|<span data-ttu-id="a2f6a-154">服务名称。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-154">A service name.</span></span>|
|<span data-ttu-id="a2f6a-155">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a2f6a-155">emailAddress</span></span>|<span data-ttu-id="a2f6a-156">String</span><span class="sxs-lookup"><span data-stu-id="a2f6a-156">String</span></span>|<span data-ttu-id="a2f6a-157">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="a2f6a-157">An email address</span></span>|
|<span data-ttu-id="a2f6a-158">id</span><span class="sxs-lookup"><span data-stu-id="a2f6a-158">id</span></span>|<span data-ttu-id="a2f6a-159">字符串</span><span class="sxs-lookup"><span data-stu-id="a2f6a-159">String</span></span>|<span data-ttu-id="a2f6a-160">该服务，以 GUID 格式的 ID。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-160">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="a2f6a-161">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-161">Read-only.</span></span>|
|<span data-ttu-id="a2f6a-162">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="a2f6a-162">isHiddenFromCustomers</span></span>|<span data-ttu-id="a2f6a-163">布尔</span><span class="sxs-lookup"><span data-stu-id="a2f6a-163">Boolean</span></span>|<span data-ttu-id="a2f6a-164">True 表示该服务不是预定的客户。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-164">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="a2f6a-165">notes</span><span class="sxs-lookup"><span data-stu-id="a2f6a-165">notes</span></span>|<span data-ttu-id="a2f6a-166">String</span><span class="sxs-lookup"><span data-stu-id="a2f6a-166">String</span></span>|<span data-ttu-id="a2f6a-167">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-167">Additional information about this service.</span></span>|
|<span data-ttu-id="a2f6a-168">后</span><span class="sxs-lookup"><span data-stu-id="a2f6a-168">postBuffer</span></span>|<span data-ttu-id="a2f6a-169">Duration</span><span class="sxs-lookup"><span data-stu-id="a2f6a-169">Duration</span></span>|<span data-ttu-id="a2f6a-170">此服务的时间为缓冲区之后为约会结束，且在下一步之前客户约会可以为预约。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-170">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="a2f6a-171">缓冲区</span><span class="sxs-lookup"><span data-stu-id="a2f6a-171">preBuffer</span></span>|<span data-ttu-id="a2f6a-172">Duration</span><span class="sxs-lookup"><span data-stu-id="a2f6a-172">Duration</span></span>|<span data-ttu-id="a2f6a-173">缓冲区之前可以启动此服务的约会的时间。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-173">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="a2f6a-174">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="a2f6a-174">schedulingPolicy</span></span>|[<span data-ttu-id="a2f6a-175">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="a2f6a-175">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="a2f6a-176">确定如何创建和管理服务此类型的约会的策略集。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-176">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="a2f6a-177">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="a2f6a-177">staffMemberIds</span></span>|<span data-ttu-id="a2f6a-178">String 集合</span><span class="sxs-lookup"><span data-stu-id="a2f6a-178">String collection</span></span>|<span data-ttu-id="a2f6a-179">表示这些[员工](bookingstaffmember.md)提供此服务。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-179">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a2f6a-180">Relationships</span><span class="sxs-lookup"><span data-stu-id="a2f6a-180">Relationships</span></span>
<span data-ttu-id="a2f6a-181">无</span><span class="sxs-lookup"><span data-stu-id="a2f6a-181">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a2f6a-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2f6a-182">JSON representation</span></span>

<span data-ttu-id="a2f6a-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2f6a-183">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
