---
title: bookingAppointment 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: f08b33cd223a140373f6130f19099ce0c941d8b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442190"
---
# <a name="bookingappointment-resource-type"></a><span data-ttu-id="979b9-104">bookingAppointment 资源类型</span><span class="sxs-lookup"><span data-stu-id="979b9-104">bookingAppointment resource type</span></span>

<span data-ttu-id="979b9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="979b9-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="979b9-106">表示由 Microsoft 记帐业务提供的一组员工执行的[bookingService](bookingservice.md)的客户约会。</span><span class="sxs-lookup"><span data-stu-id="979b9-106">Represents a customer appointment for a [bookingService](bookingservice.md), performed by a set of staff members, provided by a Microsoft Bookings business.</span></span>


## <a name="methods"></a><span data-ttu-id="979b9-107">方法</span><span class="sxs-lookup"><span data-stu-id="979b9-107">Methods</span></span>

| <span data-ttu-id="979b9-108">方法</span><span class="sxs-lookup"><span data-stu-id="979b9-108">Method</span></span>           | <span data-ttu-id="979b9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="979b9-109">Return Type</span></span>    |<span data-ttu-id="979b9-110">说明</span><span class="sxs-lookup"><span data-stu-id="979b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="979b9-111">列出约会</span><span class="sxs-lookup"><span data-stu-id="979b9-111">List appointments</span></span>](../api/bookingbusiness-list-appointments.md) |  <span data-ttu-id="979b9-112">[bookingAppointment](bookingappointment.md)集合</span><span class="sxs-lookup"><span data-stu-id="979b9-112">[bookingAppointment](bookingappointment.md) collection</span></span> | <span data-ttu-id="979b9-113">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingAppointment**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="979b9-113">Get a list of **bookingAppointment** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="979b9-114">创建 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="979b9-114">Create bookingAppointment</span></span>](../api/bookingbusiness-post-appointments.md) |  [<span data-ttu-id="979b9-115">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="979b9-115">bookingAppointment</span></span>](bookingappointment.md) | <span data-ttu-id="979b9-116">为指定的[bookingbusiness](../resources/bookingbusiness.md)创建新的**bookingAppointment** 。</span><span class="sxs-lookup"><span data-stu-id="979b9-116">Create a new **bookingAppointment** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="979b9-117">获取 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="979b9-117">Get bookingAppointment</span></span>](../api/bookingappointment-get.md) | [<span data-ttu-id="979b9-118">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="979b9-118">bookingAppointment</span></span>](bookingappointment.md) |<span data-ttu-id="979b9-119">读取**bookingAppointment**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="979b9-119">Read the properties and relationships of **bookingAppointment** object.</span></span>|
|[<span data-ttu-id="979b9-120">更新</span><span class="sxs-lookup"><span data-stu-id="979b9-120">Update</span></span>](../api/bookingappointment-update.md) | [<span data-ttu-id="979b9-121">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="979b9-121">bookingAppointment</span></span>](bookingappointment.md)    |<span data-ttu-id="979b9-122">更新**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="979b9-122">Update a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="979b9-123">删除</span><span class="sxs-lookup"><span data-stu-id="979b9-123">Delete</span></span>](../api/bookingappointment-delete.md) | <span data-ttu-id="979b9-124">无</span><span class="sxs-lookup"><span data-stu-id="979b9-124">None</span></span> |<span data-ttu-id="979b9-125">删除**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="979b9-125">Delete a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="979b9-126">Cancel</span><span class="sxs-lookup"><span data-stu-id="979b9-126">Cancel</span></span>](../api/bookingappointment-cancel.md)|<span data-ttu-id="979b9-127">无</span><span class="sxs-lookup"><span data-stu-id="979b9-127">None</span></span>| <span data-ttu-id="979b9-128">取消**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="979b9-128">Cancel a **bookingAppointment** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="979b9-129">属性</span><span class="sxs-lookup"><span data-stu-id="979b9-129">Properties</span></span>
| <span data-ttu-id="979b9-130">属性</span><span class="sxs-lookup"><span data-stu-id="979b9-130">Property</span></span>     | <span data-ttu-id="979b9-131">类型</span><span class="sxs-lookup"><span data-stu-id="979b9-131">Type</span></span>   |<span data-ttu-id="979b9-132">说明</span><span class="sxs-lookup"><span data-stu-id="979b9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="979b9-133">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="979b9-133">customerEmailAddress</span></span>|<span data-ttu-id="979b9-134">String</span><span class="sxs-lookup"><span data-stu-id="979b9-134">String</span></span>|<span data-ttu-id="979b9-135">预订约会的[bookingCustomer](bookingcustomer.md)的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="979b9-135">The SMTP address of the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="979b9-136">customerId</span><span class="sxs-lookup"><span data-stu-id="979b9-136">customerId</span></span>|<span data-ttu-id="979b9-137">String</span><span class="sxs-lookup"><span data-stu-id="979b9-137">String</span></span>|<span data-ttu-id="979b9-138">此约会的[bookingCustomer](bookingcustomer.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="979b9-138">The ID of the [bookingCustomer](bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="979b9-139">如果创建约会时未指定 ID，则会创建一个新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="979b9-139">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="979b9-140">设置后，应考虑**customerId**不可变。</span><span class="sxs-lookup"><span data-stu-id="979b9-140">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="979b9-141">customerLocation</span><span class="sxs-lookup"><span data-stu-id="979b9-141">customerLocation</span></span>|[<span data-ttu-id="979b9-142">位置</span><span class="sxs-lookup"><span data-stu-id="979b9-142">location</span></span>](location.md)|<span data-ttu-id="979b9-143">表示预订约会的[bookingCustomer](bookingcustomer.md)的位置信息。</span><span class="sxs-lookup"><span data-stu-id="979b9-143">Represents location information for the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="979b9-144">customerName</span><span class="sxs-lookup"><span data-stu-id="979b9-144">customerName</span></span>|<span data-ttu-id="979b9-145">String</span><span class="sxs-lookup"><span data-stu-id="979b9-145">String</span></span>|<span data-ttu-id="979b9-146">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="979b9-146">The customer's name.</span></span>|
|<span data-ttu-id="979b9-147">customerNotes</span><span class="sxs-lookup"><span data-stu-id="979b9-147">customerNotes</span></span>|<span data-ttu-id="979b9-148">String</span><span class="sxs-lookup"><span data-stu-id="979b9-148">String</span></span>|<span data-ttu-id="979b9-149">来自与此约会相关联的客户的注释。</span><span class="sxs-lookup"><span data-stu-id="979b9-149">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="979b9-150">仅当按 ID 读取此**bookingAppointment**时，才能获取该值。</span><span class="sxs-lookup"><span data-stu-id="979b9-150">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="979b9-151">只有在最初创建新客户的约会时，才能设置该属性。</span><span class="sxs-lookup"><span data-stu-id="979b9-151">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="979b9-152">然后，将从**customerId**表示的客户计算该值。</span><span class="sxs-lookup"><span data-stu-id="979b9-152">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="979b9-153">customerPhone</span><span class="sxs-lookup"><span data-stu-id="979b9-153">customerPhone</span></span>|<span data-ttu-id="979b9-154">String</span><span class="sxs-lookup"><span data-stu-id="979b9-154">String</span></span>|<span data-ttu-id="979b9-155">客户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="979b9-155">The customer's phone number.</span></span>|
|<span data-ttu-id="979b9-156">duration</span><span class="sxs-lookup"><span data-stu-id="979b9-156">duration</span></span>|<span data-ttu-id="979b9-157">持续时间</span><span class="sxs-lookup"><span data-stu-id="979b9-157">Duration</span></span>|<span data-ttu-id="979b9-158">约会的长度，以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="979b9-158">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="979b9-159">end</span><span class="sxs-lookup"><span data-stu-id="979b9-159">end</span></span>|[<span data-ttu-id="979b9-160">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="979b9-160">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="979b9-161">约会结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="979b9-161">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="979b9-162">id</span><span class="sxs-lookup"><span data-stu-id="979b9-162">id</span></span>|<span data-ttu-id="979b9-163">String</span><span class="sxs-lookup"><span data-stu-id="979b9-163">String</span></span>| <span data-ttu-id="979b9-164">**BookingAppointment**的 ID。</span><span class="sxs-lookup"><span data-stu-id="979b9-164">The ID of the **bookingAppointment**.</span></span> <span data-ttu-id="979b9-165">只读。</span><span class="sxs-lookup"><span data-stu-id="979b9-165">Read-only.</span></span>|
|<span data-ttu-id="979b9-166">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="979b9-166">invoiceAmount</span></span>|<span data-ttu-id="979b9-167">双精度</span><span class="sxs-lookup"><span data-stu-id="979b9-167">Double</span></span>|<span data-ttu-id="979b9-168">发票上的计费金额。</span><span class="sxs-lookup"><span data-stu-id="979b9-168">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="979b9-169">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="979b9-169">invoiceDate</span></span>|[<span data-ttu-id="979b9-170">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="979b9-170">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="979b9-171">此约会的发票的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="979b9-171">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="979b9-172">invoiceId</span><span class="sxs-lookup"><span data-stu-id="979b9-172">invoiceId</span></span>|<span data-ttu-id="979b9-173">String</span><span class="sxs-lookup"><span data-stu-id="979b9-173">String</span></span>|<span data-ttu-id="979b9-174">发票的 ID。</span><span class="sxs-lookup"><span data-stu-id="979b9-174">The ID of the invoice.</span></span>|
|<span data-ttu-id="979b9-175">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="979b9-175">invoiceStatus</span></span>|<span data-ttu-id="979b9-176">string</span><span class="sxs-lookup"><span data-stu-id="979b9-176">string</span></span>| <span data-ttu-id="979b9-177">发票的状态。</span><span class="sxs-lookup"><span data-stu-id="979b9-177">The status of the invoice.</span></span> <span data-ttu-id="979b9-178">可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="979b9-178">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="979b9-179">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="979b9-179">invoiceUrl</span></span>|<span data-ttu-id="979b9-180">String</span><span class="sxs-lookup"><span data-stu-id="979b9-180">String</span></span>|<span data-ttu-id="979b9-181">Microsoft 预订中发票的 URL。</span><span class="sxs-lookup"><span data-stu-id="979b9-181">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="979b9-182">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="979b9-182">optOutOfCustomerEmail</span></span>|<span data-ttu-id="979b9-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="979b9-183">Boolean</span></span>|<span data-ttu-id="979b9-184">如果为 True，则表示此约会的[bookingCustomer](bookingcustomer.md)不希望收到此约会的确认。</span><span class="sxs-lookup"><span data-stu-id="979b9-184">True indicates that the [bookingCustomer](bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="979b9-185">postBuffer</span><span class="sxs-lookup"><span data-stu-id="979b9-185">postBuffer</span></span>|<span data-ttu-id="979b9-186">持续时间</span><span class="sxs-lookup"><span data-stu-id="979b9-186">Duration</span></span>|<span data-ttu-id="979b9-187">在约会结束后保留的时间长度，例如，进行清理。</span><span class="sxs-lookup"><span data-stu-id="979b9-187">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="979b9-188">值以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="979b9-188">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="979b9-189">preBuffer</span><span class="sxs-lookup"><span data-stu-id="979b9-189">preBuffer</span></span>|<span data-ttu-id="979b9-190">持续时间</span><span class="sxs-lookup"><span data-stu-id="979b9-190">Duration</span></span>|<span data-ttu-id="979b9-191">在约会开始之前保留的时间量（以供准备）为例。</span><span class="sxs-lookup"><span data-stu-id="979b9-191">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="979b9-192">值以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="979b9-192">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="979b9-193">特价</span><span class="sxs-lookup"><span data-stu-id="979b9-193">price</span></span>|<span data-ttu-id="979b9-194">双精度</span><span class="sxs-lookup"><span data-stu-id="979b9-194">Double</span></span>|<span data-ttu-id="979b9-195">指定[bookingService](bookingservice.md)的约会的常规价格。</span><span class="sxs-lookup"><span data-stu-id="979b9-195">The regular price for an appointment for the specified [bookingService](bookingservice.md).</span></span>|
|<span data-ttu-id="979b9-196">priceType</span><span class="sxs-lookup"><span data-stu-id="979b9-196">priceType</span></span>|<span data-ttu-id="979b9-197">string</span><span class="sxs-lookup"><span data-stu-id="979b9-197">string</span></span>| <span data-ttu-id="979b9-198">一种设置，可为服务的定价结构提供灵活性。</span><span class="sxs-lookup"><span data-stu-id="979b9-198">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="979b9-199">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="979b9-199">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="979b9-200">提醒</span><span class="sxs-lookup"><span data-stu-id="979b9-200">reminders</span></span>|<span data-ttu-id="979b9-201">[bookingReminder](bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="979b9-201">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="979b9-202">为此约会发送的客户提醒的集合。</span><span class="sxs-lookup"><span data-stu-id="979b9-202">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="979b9-203">此属性的值仅在按 ID 读取此**bookingAppointment**时可用。</span><span class="sxs-lookup"><span data-stu-id="979b9-203">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="979b9-204">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="979b9-204">selfServiceAppointmentId</span></span>|<span data-ttu-id="979b9-205">String</span><span class="sxs-lookup"><span data-stu-id="979b9-205">String</span></span>|<span data-ttu-id="979b9-206">约会的其他跟踪 ID，如果约会是由客户在日程安排页面上直接创建的，而不是代表客户由教职员工成员创建的。</span><span class="sxs-lookup"><span data-stu-id="979b9-206">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="979b9-207">服务 Id</span><span class="sxs-lookup"><span data-stu-id="979b9-207">serviceId</span></span>|<span data-ttu-id="979b9-208">String</span><span class="sxs-lookup"><span data-stu-id="979b9-208">String</span></span>|<span data-ttu-id="979b9-209">与此约会相关联的[bookingService](bookingservice.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="979b9-209">The ID of the [bookingService](bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="979b9-210">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="979b9-210">serviceLocation</span></span>|[<span data-ttu-id="979b9-211">位置</span><span class="sxs-lookup"><span data-stu-id="979b9-211">location</span></span>](location.md)|<span data-ttu-id="979b9-212">服务的传递位置。</span><span class="sxs-lookup"><span data-stu-id="979b9-212">The location where the service is delivered.</span></span>|
|<span data-ttu-id="979b9-213">serviceName</span><span class="sxs-lookup"><span data-stu-id="979b9-213">serviceName</span></span>|<span data-ttu-id="979b9-214">String</span><span class="sxs-lookup"><span data-stu-id="979b9-214">String</span></span>|<span data-ttu-id="979b9-215">与此约会相关联的**bookingService**的名称。</span><span class="sxs-lookup"><span data-stu-id="979b9-215">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="979b9-216">创建新约会时，此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="979b9-216">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="979b9-217">如果未指定，则通过**serviceId**属性从与约会关联的服务计算。</span><span class="sxs-lookup"><span data-stu-id="979b9-217">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="979b9-218">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="979b9-218">serviceNotes</span></span>|<span data-ttu-id="979b9-219">String</span><span class="sxs-lookup"><span data-stu-id="979b9-219">String</span></span>|<span data-ttu-id="979b9-220">来自[bookingStaffMember](bookingstaffmember.md)的注释。</span><span class="sxs-lookup"><span data-stu-id="979b9-220">Notes from a [bookingStaffMember](bookingstaffmember.md).</span></span> <span data-ttu-id="979b9-221">此属性的值仅在按 ID 读取此**bookingAppointment**时可用。</span><span class="sxs-lookup"><span data-stu-id="979b9-221">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="979b9-222">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="979b9-222">staffMemberIds</span></span>|<span data-ttu-id="979b9-223">String 集合</span><span class="sxs-lookup"><span data-stu-id="979b9-223">String collection</span></span>|<span data-ttu-id="979b9-224">在此约会中计划的每个[bookingStaffMember](bookingstaffmember.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="979b9-224">The ID of each [bookingStaffMember](bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="979b9-225">start</span><span class="sxs-lookup"><span data-stu-id="979b9-225">start</span></span>|[<span data-ttu-id="979b9-226">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="979b9-226">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="979b9-227">约会开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="979b9-227">The date, time, and time zone that the appointment begins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="979b9-228">关系</span><span class="sxs-lookup"><span data-stu-id="979b9-228">Relationships</span></span>
<span data-ttu-id="979b9-229">无</span><span class="sxs-lookup"><span data-stu-id="979b9-229">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="979b9-230">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="979b9-230">JSON representation</span></span>

<span data-ttu-id="979b9-231">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="979b9-231">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingAppointment"
}-->

```json
{
  "customerEmailAddress": "String",
  "customerId": "String",
  "customerLocation": {"@odata.type": "microsoft.graph.location"},
  "customerName": "String",
  "customerNotes": "String",
  "customerPhone": "String",
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "optOutOfCustomerEmail": true,
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": "string",
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
