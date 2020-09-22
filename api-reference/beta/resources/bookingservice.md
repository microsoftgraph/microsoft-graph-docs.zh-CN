---
title: bookingService 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 37a1e6adb6a4769601d5f9806d1e3b262fe2879f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071743"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="d2dbb-104">bookingService 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2dbb-104">bookingService resource type</span></span>

<span data-ttu-id="d2dbb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2dbb-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d2dbb-106">表示有关 [bookingBusiness](bookingbusiness.md)提供的特定服务的信息，如服务名称、价格和通常提供此类服务的人员。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-106">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="d2dbb-107">方法</span><span class="sxs-lookup"><span data-stu-id="d2dbb-107">Methods</span></span>

| <span data-ttu-id="d2dbb-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2dbb-108">Method</span></span>           | <span data-ttu-id="d2dbb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2dbb-109">Return Type</span></span>    |<span data-ttu-id="d2dbb-110">说明</span><span class="sxs-lookup"><span data-stu-id="d2dbb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2dbb-111">列出服务</span><span class="sxs-lookup"><span data-stu-id="d2dbb-111">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="d2dbb-112">[bookingService](bookingservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2dbb-112">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="d2dbb-113">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-113">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="d2dbb-114">创建 bookingService</span><span class="sxs-lookup"><span data-stu-id="d2dbb-114">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="d2dbb-115">bookingService</span><span class="sxs-lookup"><span data-stu-id="d2dbb-115">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="d2dbb-116">为指定的[bookingbusiness](../resources/bookingbusiness.md)创建**bookingService** 。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-116">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="d2dbb-117">获取 bookingService</span><span class="sxs-lookup"><span data-stu-id="d2dbb-117">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="d2dbb-118">bookingService</span><span class="sxs-lookup"><span data-stu-id="d2dbb-118">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="d2dbb-119">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-119">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="d2dbb-120">更新</span><span class="sxs-lookup"><span data-stu-id="d2dbb-120">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="d2dbb-121">bookingService</span><span class="sxs-lookup"><span data-stu-id="d2dbb-121">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="d2dbb-122">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-122">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="d2dbb-123">删除</span><span class="sxs-lookup"><span data-stu-id="d2dbb-123">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="d2dbb-124">无</span><span class="sxs-lookup"><span data-stu-id="d2dbb-124">None</span></span> |<span data-ttu-id="d2dbb-125">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-125">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="d2dbb-126">属性</span><span class="sxs-lookup"><span data-stu-id="d2dbb-126">Properties</span></span>
| <span data-ttu-id="d2dbb-127">属性</span><span class="sxs-lookup"><span data-stu-id="d2dbb-127">Property</span></span>     | <span data-ttu-id="d2dbb-128">类型</span><span class="sxs-lookup"><span data-stu-id="d2dbb-128">Type</span></span>   |<span data-ttu-id="d2dbb-129">说明</span><span class="sxs-lookup"><span data-stu-id="d2dbb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2dbb-130">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="d2dbb-130">defaultDuration</span></span>|<span data-ttu-id="d2dbb-131">持续时间</span><span class="sxs-lookup"><span data-stu-id="d2dbb-131">Duration</span></span>|<span data-ttu-id="d2dbb-132">服务的默认长度，以天数、小时数、分钟数和秒数表示。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-132">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="d2dbb-133">例如，P11D23H59M 59.999999999999 S。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-133">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="d2dbb-134">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="d2dbb-134">defaultLocation</span></span>|[<span data-ttu-id="d2dbb-135">location</span><span class="sxs-lookup"><span data-stu-id="d2dbb-135">location</span></span>](location.md)|<span data-ttu-id="d2dbb-136">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-136">The default physical location for the service.</span></span>|
|<span data-ttu-id="d2dbb-137">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="d2dbb-137">defaultPrice</span></span>|<span data-ttu-id="d2dbb-138">双精度</span><span class="sxs-lookup"><span data-stu-id="d2dbb-138">Double</span></span>|<span data-ttu-id="d2dbb-139">服务的默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-139">The default monetary price for the service.</span></span>|
|<span data-ttu-id="d2dbb-140">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="d2dbb-140">defaultPriceType</span></span>|<span data-ttu-id="d2dbb-141">string</span><span class="sxs-lookup"><span data-stu-id="d2dbb-141">string</span></span>|<span data-ttu-id="d2dbb-142">服务收费的默认方式。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-142">The default way the service is charged.</span></span> <span data-ttu-id="d2dbb-143">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-143">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="d2dbb-144">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="d2dbb-144">defaultReminders</span></span>|<span data-ttu-id="d2dbb-145">[bookingReminder](bookingreminder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2dbb-145">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="d2dbb-146">此服务的约会的默认提醒集。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-146">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="d2dbb-147">此属性的值仅在按 ID 读取此 **bookingService** 时可用。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-147">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="d2dbb-148">说明</span><span class="sxs-lookup"><span data-stu-id="d2dbb-148">description</span></span>|<span data-ttu-id="d2dbb-149">String</span><span class="sxs-lookup"><span data-stu-id="d2dbb-149">String</span></span>|<span data-ttu-id="d2dbb-150">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-150">A text description for the service.</span></span>|
|<span data-ttu-id="d2dbb-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d2dbb-151">displayName</span></span>|<span data-ttu-id="d2dbb-152">String</span><span class="sxs-lookup"><span data-stu-id="d2dbb-152">String</span></span>|<span data-ttu-id="d2dbb-153">服务名称。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-153">A service name.</span></span>|
|<span data-ttu-id="d2dbb-154">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d2dbb-154">emailAddress</span></span>|<span data-ttu-id="d2dbb-155">String</span><span class="sxs-lookup"><span data-stu-id="d2dbb-155">String</span></span>|<span data-ttu-id="d2dbb-156">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="d2dbb-156">An email address</span></span>|
|<span data-ttu-id="d2dbb-157">id</span><span class="sxs-lookup"><span data-stu-id="d2dbb-157">id</span></span>|<span data-ttu-id="d2dbb-158">String</span><span class="sxs-lookup"><span data-stu-id="d2dbb-158">String</span></span>|<span data-ttu-id="d2dbb-159">该服务的 ID （采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-159">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="d2dbb-160">只读。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-160">Read-only.</span></span>|
|<span data-ttu-id="d2dbb-161">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="d2dbb-161">isHiddenFromCustomers</span></span>|<span data-ttu-id="d2dbb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2dbb-162">Boolean</span></span>|<span data-ttu-id="d2dbb-163">如果为 True，则表示此服务不可供客户预订。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-163">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="d2dbb-164">notes</span><span class="sxs-lookup"><span data-stu-id="d2dbb-164">notes</span></span>|<span data-ttu-id="d2dbb-165">String</span><span class="sxs-lookup"><span data-stu-id="d2dbb-165">String</span></span>|<span data-ttu-id="d2dbb-166">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-166">Additional information about this service.</span></span>|
|<span data-ttu-id="d2dbb-167">postBuffer</span><span class="sxs-lookup"><span data-stu-id="d2dbb-167">postBuffer</span></span>|<span data-ttu-id="d2dbb-168">持续时间</span><span class="sxs-lookup"><span data-stu-id="d2dbb-168">Duration</span></span>|<span data-ttu-id="d2dbb-169">此服务的约会结束后以及下一个客户约会可以被预订前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-169">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="d2dbb-170">preBuffer</span><span class="sxs-lookup"><span data-stu-id="d2dbb-170">preBuffer</span></span>|<span data-ttu-id="d2dbb-171">持续时间</span><span class="sxs-lookup"><span data-stu-id="d2dbb-171">Duration</span></span>|<span data-ttu-id="d2dbb-172">在此服务的约会开始之前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-172">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="d2dbb-173">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="d2dbb-173">schedulingPolicy</span></span>|[<span data-ttu-id="d2dbb-174">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="d2dbb-174">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="d2dbb-175">确定应如何创建和管理此类服务的约会的一组策略。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-175">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="d2dbb-176">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="d2dbb-176">staffMemberIds</span></span>|<span data-ttu-id="d2dbb-177">String 集合</span><span class="sxs-lookup"><span data-stu-id="d2dbb-177">String collection</span></span>|<span data-ttu-id="d2dbb-178">代表提供此服务的 [教职员工成员](bookingstaffmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-178">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d2dbb-179">关系</span><span class="sxs-lookup"><span data-stu-id="d2dbb-179">Relationships</span></span>
<span data-ttu-id="d2dbb-180">无</span><span class="sxs-lookup"><span data-stu-id="d2dbb-180">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d2dbb-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2dbb-181">JSON representation</span></span>

<span data-ttu-id="d2dbb-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2dbb-182">The following is a JSON representation of the resource.</span></span>

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


