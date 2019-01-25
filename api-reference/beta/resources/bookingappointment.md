---
title: bookingAppointment 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c5868788159f0602c1f8a263138c7ce9107c2c94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509838"
---
# <a name="bookingappointment-resource-type"></a><span data-ttu-id="a6eb0-104">bookingAppointment 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6eb0-104">bookingAppointment resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="a6eb0-105">代表[bookingService](bookingservice.md)，由一组人员成员，由 Microsoft 预订业务执行客户约会。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-105">Represents a customer appointment for a [bookingService](bookingservice.md), performed by a set of staff members, provided by a Microsoft Bookings business.</span></span>


## <a name="methods"></a><span data-ttu-id="a6eb0-106">方法</span><span class="sxs-lookup"><span data-stu-id="a6eb0-106">Methods</span></span>

| <span data-ttu-id="a6eb0-107">方法</span><span class="sxs-lookup"><span data-stu-id="a6eb0-107">Method</span></span>           | <span data-ttu-id="a6eb0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6eb0-108">Return Type</span></span>    |<span data-ttu-id="a6eb0-109">说明</span><span class="sxs-lookup"><span data-stu-id="a6eb0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6eb0-110">列表约会</span><span class="sxs-lookup"><span data-stu-id="a6eb0-110">List appointments</span></span>](../api/bookingbusiness-list-appointments.md) |  <span data-ttu-id="a6eb0-111">[bookingAppointment](bookingappointment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6eb0-111">[bookingAppointment](bookingappointment.md) collection</span></span> | <span data-ttu-id="a6eb0-112">指定[bookingbusiness](../resources/bookingbusiness.md)中获取**bookingAppointment**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-112">Get a list of **bookingAppointment** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="a6eb0-113">创建 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="a6eb0-113">Create bookingAppointment</span></span>](../api/bookingbusiness-post-appointments.md) |  [<span data-ttu-id="a6eb0-114">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="a6eb0-114">bookingAppointment</span></span>](bookingappointment.md) | <span data-ttu-id="a6eb0-115">创建新**bookingAppointment**的指定[bookingbusiness](../resources/bookingbusiness.md)。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-115">Create a new **bookingAppointment** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="a6eb0-116">获取 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="a6eb0-116">Get bookingAppointment</span></span>](../api/bookingappointment-get.md) | [<span data-ttu-id="a6eb0-117">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="a6eb0-117">bookingAppointment</span></span>](bookingappointment.md) |<span data-ttu-id="a6eb0-118">读取的属性和**bookingAppointment**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-118">Read the properties and relationships of **bookingAppointment** object.</span></span>|
|[<span data-ttu-id="a6eb0-119">Update</span><span class="sxs-lookup"><span data-stu-id="a6eb0-119">Update</span></span>](../api/bookingappointment-update.md) | [<span data-ttu-id="a6eb0-120">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="a6eb0-120">bookingAppointment</span></span>](bookingappointment.md)    |<span data-ttu-id="a6eb0-121">更新**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-121">Update a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="a6eb0-122">删除</span><span class="sxs-lookup"><span data-stu-id="a6eb0-122">Delete</span></span>](../api/bookingappointment-delete.md) | <span data-ttu-id="a6eb0-123">无</span><span class="sxs-lookup"><span data-stu-id="a6eb0-123">None</span></span> |<span data-ttu-id="a6eb0-124">删除**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-124">Delete a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="a6eb0-125">Cancel</span><span class="sxs-lookup"><span data-stu-id="a6eb0-125">Cancel</span></span>](../api/bookingappointment-cancel.md)|<span data-ttu-id="a6eb0-126">无</span><span class="sxs-lookup"><span data-stu-id="a6eb0-126">None</span></span>| <span data-ttu-id="a6eb0-127">取消**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-127">Cancel a **bookingAppointment** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6eb0-128">属性</span><span class="sxs-lookup"><span data-stu-id="a6eb0-128">Properties</span></span>
| <span data-ttu-id="a6eb0-129">属性</span><span class="sxs-lookup"><span data-stu-id="a6eb0-129">Property</span></span>     | <span data-ttu-id="a6eb0-130">类型</span><span class="sxs-lookup"><span data-stu-id="a6eb0-130">Type</span></span>   |<span data-ttu-id="a6eb0-131">说明</span><span class="sxs-lookup"><span data-stu-id="a6eb0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6eb0-132">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a6eb0-132">customerEmailAddress</span></span>|<span data-ttu-id="a6eb0-133">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-133">String</span></span>|<span data-ttu-id="a6eb0-134">预订约会[bookingCustomer](bookingcustomer.md) SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-134">The SMTP address of the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="a6eb0-135">customerId</span><span class="sxs-lookup"><span data-stu-id="a6eb0-135">customerId</span></span>|<span data-ttu-id="a6eb0-136">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-136">String</span></span>|<span data-ttu-id="a6eb0-137">该约会的[bookingCustomer](bookingcustomer.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-137">The ID of the [bookingCustomer](bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="a6eb0-138">如果未指定 ID 创建约会时，将创建一个新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-138">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="a6eb0-139">设置后，您应考虑**customerId**变。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-139">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="a6eb0-140">customerLocation</span><span class="sxs-lookup"><span data-stu-id="a6eb0-140">customerLocation</span></span>|[<span data-ttu-id="a6eb0-141">location</span><span class="sxs-lookup"><span data-stu-id="a6eb0-141">location</span></span>](location.md)|<span data-ttu-id="a6eb0-142">代表[bookingCustomer](bookingcustomer.md)预订约会的位置信息。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-142">Represents location information for the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="a6eb0-143">customerName</span><span class="sxs-lookup"><span data-stu-id="a6eb0-143">customerName</span></span>|<span data-ttu-id="a6eb0-144">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-144">String</span></span>|<span data-ttu-id="a6eb0-145">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-145">The customer's name.</span></span>|
|<span data-ttu-id="a6eb0-146">customerNotes</span><span class="sxs-lookup"><span data-stu-id="a6eb0-146">customerNotes</span></span>|<span data-ttu-id="a6eb0-147">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-147">String</span></span>|<span data-ttu-id="a6eb0-148">从与此约会关联的客户的备注。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-148">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="a6eb0-149">您可以获取仅当读取此**bookingAppointment**其 id 值</span><span class="sxs-lookup"><span data-stu-id="a6eb0-149">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="a6eb0-150">仅在最初使用新的客户创建约会时，您可以设置该属性。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-150">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="a6eb0-151">此时，从由**customerId**客户计算的值。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-151">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="a6eb0-152">customerPhone</span><span class="sxs-lookup"><span data-stu-id="a6eb0-152">customerPhone</span></span>|<span data-ttu-id="a6eb0-153">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-153">String</span></span>|<span data-ttu-id="a6eb0-154">客户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-154">The customer's phone number.</span></span>|
|<span data-ttu-id="a6eb0-155">duration</span><span class="sxs-lookup"><span data-stu-id="a6eb0-155">duration</span></span>|<span data-ttu-id="a6eb0-156">持续时间</span><span class="sxs-lookup"><span data-stu-id="a6eb0-156">Duration</span></span>|<span data-ttu-id="a6eb0-157">约会中[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式的长度。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-157">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="a6eb0-158">end</span><span class="sxs-lookup"><span data-stu-id="a6eb0-158">end</span></span>|[<span data-ttu-id="a6eb0-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a6eb0-159">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a6eb0-160">日期、 时间和约会的结束的时区。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-160">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="a6eb0-161">id</span><span class="sxs-lookup"><span data-stu-id="a6eb0-161">id</span></span>|<span data-ttu-id="a6eb0-162">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-162">String</span></span>| <span data-ttu-id="a6eb0-163">**BookingAppointment**的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-163">The ID of the **bookingAppointment**.</span></span> <span data-ttu-id="a6eb0-164">只读。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-164">Read-only.</span></span>|
|<span data-ttu-id="a6eb0-165">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="a6eb0-165">invoiceAmount</span></span>|<span data-ttu-id="a6eb0-166">双精度</span><span class="sxs-lookup"><span data-stu-id="a6eb0-166">Double</span></span>|<span data-ttu-id="a6eb0-167">记帐的发票量。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-167">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="a6eb0-168">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="a6eb0-168">invoiceDate</span></span>|[<span data-ttu-id="a6eb0-169">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a6eb0-169">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a6eb0-170">日期、 时间和此约会的发票的时区。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-170">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="a6eb0-171">invoiceId</span><span class="sxs-lookup"><span data-stu-id="a6eb0-171">invoiceId</span></span>|<span data-ttu-id="a6eb0-172">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-172">String</span></span>|<span data-ttu-id="a6eb0-173">发票的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-173">The ID of the invoice.</span></span>|
|<span data-ttu-id="a6eb0-174">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="a6eb0-174">invoiceStatus</span></span>|<span data-ttu-id="a6eb0-175">string</span><span class="sxs-lookup"><span data-stu-id="a6eb0-175">string</span></span>| <span data-ttu-id="a6eb0-176">发票的状态。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-176">The status of the invoice.</span></span> <span data-ttu-id="a6eb0-177">可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-177">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="a6eb0-178">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="a6eb0-178">invoiceUrl</span></span>|<span data-ttu-id="a6eb0-179">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-179">String</span></span>|<span data-ttu-id="a6eb0-180">在 Microsoft 预订发票的 URL。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-180">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="a6eb0-181">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="a6eb0-181">optOutOfCustomerEmail</span></span>|<span data-ttu-id="a6eb0-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6eb0-182">Boolean</span></span>|<span data-ttu-id="a6eb0-183">True 表示该约会的[bookingCustomer](bookingcustomer.md)不希望接收该约会的确认。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-183">True indicates that the [bookingCustomer](bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="a6eb0-184">后</span><span class="sxs-lookup"><span data-stu-id="a6eb0-184">postBuffer</span></span>|<span data-ttu-id="a6eb0-185">持续时间</span><span class="sxs-lookup"><span data-stu-id="a6eb0-185">Duration</span></span>|<span data-ttu-id="a6eb0-186">保留后的清理，例如约会结束的时间量。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-186">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="a6eb0-187">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-187">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="a6eb0-188">缓冲区</span><span class="sxs-lookup"><span data-stu-id="a6eb0-188">preBuffer</span></span>|<span data-ttu-id="a6eb0-189">持续时间</span><span class="sxs-lookup"><span data-stu-id="a6eb0-189">Duration</span></span>|<span data-ttu-id="a6eb0-190">保留之前的准备，例如约会开始的时间量。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-190">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="a6eb0-191">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-191">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="a6eb0-192">Price</span><span class="sxs-lookup"><span data-stu-id="a6eb0-192">price</span></span>|<span data-ttu-id="a6eb0-193">双精度</span><span class="sxs-lookup"><span data-stu-id="a6eb0-193">Double</span></span>|<span data-ttu-id="a6eb0-194">指定[bookingService](bookingservice.md)约会正则价格。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-194">The regular price for an appointment for the specified [bookingService](bookingservice.md).</span></span>|
|<span data-ttu-id="a6eb0-195">priceType</span><span class="sxs-lookup"><span data-stu-id="a6eb0-195">priceType</span></span>|<span data-ttu-id="a6eb0-196">string</span><span class="sxs-lookup"><span data-stu-id="a6eb0-196">string</span></span>| <span data-ttu-id="a6eb0-197">为服务定价结构提供灵活性设置。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-197">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="a6eb0-198">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-198">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="a6eb0-199">提醒</span><span class="sxs-lookup"><span data-stu-id="a6eb0-199">reminders</span></span>|<span data-ttu-id="a6eb0-200">[bookingReminder](bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6eb0-200">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="a6eb0-201">客户提醒发送该约会的集合。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-201">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="a6eb0-202">此属性的值时，可仅读取此**bookingAppointment**由其 id。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-202">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="a6eb0-203">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="a6eb0-203">selfServiceAppointmentId</span></span>|<span data-ttu-id="a6eb0-204">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-204">String</span></span>|<span data-ttu-id="a6eb0-205">约会，如果约会的已创建直接通过计划页上的客户而不是由员工成员客户替的其他跟踪 ID。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-205">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="a6eb0-206">服务 Id</span><span class="sxs-lookup"><span data-stu-id="a6eb0-206">serviceId</span></span>|<span data-ttu-id="a6eb0-207">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-207">String</span></span>|<span data-ttu-id="a6eb0-208">与此约会相关联的[bookingService](bookingservice.md) ID。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-208">The ID of the [bookingService](bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="a6eb0-209">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="a6eb0-209">serviceLocation</span></span>|[<span data-ttu-id="a6eb0-210">location</span><span class="sxs-lookup"><span data-stu-id="a6eb0-210">location</span></span>](location.md)|<span data-ttu-id="a6eb0-211">传递服务的位置的位置。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-211">The location where the service is delivered.</span></span>|
|<span data-ttu-id="a6eb0-212">service_name</span><span class="sxs-lookup"><span data-stu-id="a6eb0-212">serviceName</span></span>|<span data-ttu-id="a6eb0-213">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-213">String</span></span>|<span data-ttu-id="a6eb0-214">与此约会关联**bookingService**的名称。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-214">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="a6eb0-215">创建一个新的约会时，此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-215">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="a6eb0-216">如果未指定，它是从与约会**serviceId**属性关联的服务进行计算。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-216">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="a6eb0-217">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="a6eb0-217">serviceNotes</span></span>|<span data-ttu-id="a6eb0-218">String</span><span class="sxs-lookup"><span data-stu-id="a6eb0-218">String</span></span>|<span data-ttu-id="a6eb0-219">从[bookingStaffMember](bookingstaffmember.md)备注。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-219">Notes from a [bookingStaffMember](bookingstaffmember.md).</span></span> <span data-ttu-id="a6eb0-220">此属性的值时，可仅读取此**bookingAppointment**由其 id。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-220">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="a6eb0-221">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="a6eb0-221">staffMemberIds</span></span>|<span data-ttu-id="a6eb0-222">String 集合</span><span class="sxs-lookup"><span data-stu-id="a6eb0-222">String collection</span></span>|<span data-ttu-id="a6eb0-223">每个[bookingStaffMember](bookingstaffmember.md)此约会中安排的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-223">The ID of each [bookingStaffMember](bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="a6eb0-224">start</span><span class="sxs-lookup"><span data-stu-id="a6eb0-224">start</span></span>|[<span data-ttu-id="a6eb0-225">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a6eb0-225">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a6eb0-226">日期、 时间和时区约会的开始。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-226">The date, time, and time zone that the appointment begins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6eb0-227">关系</span><span class="sxs-lookup"><span data-stu-id="a6eb0-227">Relationships</span></span>
<span data-ttu-id="a6eb0-228">无</span><span class="sxs-lookup"><span data-stu-id="a6eb0-228">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a6eb0-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6eb0-229">JSON representation</span></span>

<span data-ttu-id="a6eb0-230">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6eb0-230">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingappointment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
