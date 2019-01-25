---
title: bookingService 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519883"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="9751e-104">bookingService 资源类型</span><span class="sxs-lookup"><span data-stu-id="9751e-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="9751e-105">代表由[bookingBusiness](bookingbusiness.md)，如的服务名称、 价格和通常提供了此类服务的人员提供的特定服务的信息。</span><span class="sxs-lookup"><span data-stu-id="9751e-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="9751e-106">方法</span><span class="sxs-lookup"><span data-stu-id="9751e-106">Methods</span></span>

| <span data-ttu-id="9751e-107">方法</span><span class="sxs-lookup"><span data-stu-id="9751e-107">Method</span></span>           | <span data-ttu-id="9751e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9751e-108">Return Type</span></span>    |<span data-ttu-id="9751e-109">说明</span><span class="sxs-lookup"><span data-stu-id="9751e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9751e-110">列表服务</span><span class="sxs-lookup"><span data-stu-id="9751e-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="9751e-111">[bookingService](bookingservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="9751e-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="9751e-112">指定[bookingbusiness](../resources/bookingbusiness.md)中获取**bookingService**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9751e-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="9751e-113">创建 bookingService</span><span class="sxs-lookup"><span data-stu-id="9751e-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="9751e-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="9751e-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="9751e-115">创建用于指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService** 。</span><span class="sxs-lookup"><span data-stu-id="9751e-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="9751e-116">获取 bookingService</span><span class="sxs-lookup"><span data-stu-id="9751e-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="9751e-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="9751e-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="9751e-118">指定[bookingbusiness](../resources/bookingbusiness.md)中获取的属性和**bookingService**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9751e-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="9751e-119">Update</span><span class="sxs-lookup"><span data-stu-id="9751e-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="9751e-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="9751e-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="9751e-121">更新中指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService**对象。</span><span class="sxs-lookup"><span data-stu-id="9751e-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="9751e-122">删除</span><span class="sxs-lookup"><span data-stu-id="9751e-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="9751e-123">无</span><span class="sxs-lookup"><span data-stu-id="9751e-123">None</span></span> |<span data-ttu-id="9751e-124">删除在指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService**对象。</span><span class="sxs-lookup"><span data-stu-id="9751e-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="9751e-125">属性</span><span class="sxs-lookup"><span data-stu-id="9751e-125">Properties</span></span>
| <span data-ttu-id="9751e-126">属性</span><span class="sxs-lookup"><span data-stu-id="9751e-126">Property</span></span>     | <span data-ttu-id="9751e-127">类型</span><span class="sxs-lookup"><span data-stu-id="9751e-127">Type</span></span>   |<span data-ttu-id="9751e-128">说明</span><span class="sxs-lookup"><span data-stu-id="9751e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9751e-129">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="9751e-129">defaultDuration</span></span>|<span data-ttu-id="9751e-130">持续时间</span><span class="sxs-lookup"><span data-stu-id="9751e-130">Duration</span></span>|<span data-ttu-id="9751e-131">默认服务中的天、 小时、 分钟和秒数字表示的长度。</span><span class="sxs-lookup"><span data-stu-id="9751e-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="9751e-132">例如，P11D23H59M59.999999999999S。</span><span class="sxs-lookup"><span data-stu-id="9751e-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="9751e-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="9751e-133">defaultLocation</span></span>|[<span data-ttu-id="9751e-134">location</span><span class="sxs-lookup"><span data-stu-id="9751e-134">location</span></span>](location.md)|<span data-ttu-id="9751e-135">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="9751e-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="9751e-136">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="9751e-136">defaultPrice</span></span>|<span data-ttu-id="9751e-137">双精度</span><span class="sxs-lookup"><span data-stu-id="9751e-137">Double</span></span>|<span data-ttu-id="9751e-138">该服务默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="9751e-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="9751e-139">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="9751e-139">defaultPriceType</span></span>|<span data-ttu-id="9751e-140">string</span><span class="sxs-lookup"><span data-stu-id="9751e-140">string</span></span>|<span data-ttu-id="9751e-141">负责服务的默认方式。</span><span class="sxs-lookup"><span data-stu-id="9751e-141">The default way the service is charged.</span></span> <span data-ttu-id="9751e-142">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="9751e-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="9751e-143">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="9751e-143">defaultReminders</span></span>|<span data-ttu-id="9751e-144">[bookingReminder](bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="9751e-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="9751e-145">默认设置的该服务的约会的提醒。</span><span class="sxs-lookup"><span data-stu-id="9751e-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="9751e-146">此属性的值时，可仅读取此**bookingService**由其 id。</span><span class="sxs-lookup"><span data-stu-id="9751e-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="9751e-147">说明</span><span class="sxs-lookup"><span data-stu-id="9751e-147">description</span></span>|<span data-ttu-id="9751e-148">字符串</span><span class="sxs-lookup"><span data-stu-id="9751e-148">String</span></span>|<span data-ttu-id="9751e-149">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="9751e-149">A text description for the service.</span></span>|
|<span data-ttu-id="9751e-150">displayName</span><span class="sxs-lookup"><span data-stu-id="9751e-150">displayName</span></span>|<span data-ttu-id="9751e-151">String</span><span class="sxs-lookup"><span data-stu-id="9751e-151">String</span></span>|<span data-ttu-id="9751e-152">服务名称。</span><span class="sxs-lookup"><span data-stu-id="9751e-152">A service name.</span></span>|
|<span data-ttu-id="9751e-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9751e-153">emailAddress</span></span>|<span data-ttu-id="9751e-154">String</span><span class="sxs-lookup"><span data-stu-id="9751e-154">String</span></span>|<span data-ttu-id="9751e-155">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="9751e-155">An email address</span></span>|
|<span data-ttu-id="9751e-156">id</span><span class="sxs-lookup"><span data-stu-id="9751e-156">id</span></span>|<span data-ttu-id="9751e-157">字串符号</span><span class="sxs-lookup"><span data-stu-id="9751e-157">String</span></span>|<span data-ttu-id="9751e-158">该服务，以 GUID 格式的 ID。</span><span class="sxs-lookup"><span data-stu-id="9751e-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="9751e-159">只读。</span><span class="sxs-lookup"><span data-stu-id="9751e-159">Read-only.</span></span>|
|<span data-ttu-id="9751e-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="9751e-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="9751e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9751e-161">Boolean</span></span>|<span data-ttu-id="9751e-162">True 表示该服务不是预定的客户。</span><span class="sxs-lookup"><span data-stu-id="9751e-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="9751e-163">notes</span><span class="sxs-lookup"><span data-stu-id="9751e-163">notes</span></span>|<span data-ttu-id="9751e-164">String</span><span class="sxs-lookup"><span data-stu-id="9751e-164">String</span></span>|<span data-ttu-id="9751e-165">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="9751e-165">Additional information about this service.</span></span>|
|<span data-ttu-id="9751e-166">后</span><span class="sxs-lookup"><span data-stu-id="9751e-166">postBuffer</span></span>|<span data-ttu-id="9751e-167">持续时间</span><span class="sxs-lookup"><span data-stu-id="9751e-167">Duration</span></span>|<span data-ttu-id="9751e-168">此服务的时间为缓冲区之后为约会结束，且在下一步之前客户约会可以为预约。</span><span class="sxs-lookup"><span data-stu-id="9751e-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="9751e-169">缓冲区</span><span class="sxs-lookup"><span data-stu-id="9751e-169">preBuffer</span></span>|<span data-ttu-id="9751e-170">持续时间</span><span class="sxs-lookup"><span data-stu-id="9751e-170">Duration</span></span>|<span data-ttu-id="9751e-171">缓冲区之前可以启动此服务的约会的时间。</span><span class="sxs-lookup"><span data-stu-id="9751e-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="9751e-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="9751e-172">schedulingPolicy</span></span>|[<span data-ttu-id="9751e-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="9751e-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="9751e-174">确定如何创建和管理服务此类型的约会的策略集。</span><span class="sxs-lookup"><span data-stu-id="9751e-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="9751e-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="9751e-175">staffMemberIds</span></span>|<span data-ttu-id="9751e-176">String 集合</span><span class="sxs-lookup"><span data-stu-id="9751e-176">String collection</span></span>|<span data-ttu-id="9751e-177">表示这些[员工](bookingstaffmember.md)提供此服务。</span><span class="sxs-lookup"><span data-stu-id="9751e-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9751e-178">关系</span><span class="sxs-lookup"><span data-stu-id="9751e-178">Relationships</span></span>
<span data-ttu-id="9751e-179">无</span><span class="sxs-lookup"><span data-stu-id="9751e-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9751e-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9751e-180">JSON representation</span></span>

<span data-ttu-id="9751e-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9751e-181">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
