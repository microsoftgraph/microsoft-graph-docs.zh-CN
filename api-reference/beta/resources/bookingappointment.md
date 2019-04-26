---
title: bookingAppointment 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 8b1d481d43374d8611f221fb5c3047cdc9cd9148
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328222"
---
# <a name="bookingappointment-resource-type"></a><span data-ttu-id="0e248-104">bookingAppointment 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e248-104">bookingAppointment resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="0e248-105">表示由 Microsoft 记帐业务提供的一组员工执行的[bookingService](bookingservice.md)的客户约会。</span><span class="sxs-lookup"><span data-stu-id="0e248-105">Represents a customer appointment for a [bookingService](bookingservice.md), performed by a set of staff members, provided by a Microsoft Bookings business.</span></span>


## <a name="methods"></a><span data-ttu-id="0e248-106">方法</span><span class="sxs-lookup"><span data-stu-id="0e248-106">Methods</span></span>

| <span data-ttu-id="0e248-107">方法</span><span class="sxs-lookup"><span data-stu-id="0e248-107">Method</span></span>           | <span data-ttu-id="0e248-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e248-108">Return Type</span></span>    |<span data-ttu-id="0e248-109">说明</span><span class="sxs-lookup"><span data-stu-id="0e248-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e248-110">列出约会</span><span class="sxs-lookup"><span data-stu-id="0e248-110">List appointments</span></span>](../api/bookingbusiness-list-appointments.md) |  <span data-ttu-id="0e248-111">[bookingAppointment](bookingappointment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e248-111">[bookingAppointment](bookingappointment.md) collection</span></span> | <span data-ttu-id="0e248-112">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingAppointment**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0e248-112">Get a list of **bookingAppointment** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="0e248-113">创建 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="0e248-113">Create bookingAppointment</span></span>](../api/bookingbusiness-post-appointments.md) |  [<span data-ttu-id="0e248-114">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="0e248-114">bookingAppointment</span></span>](bookingappointment.md) | <span data-ttu-id="0e248-115">为指定的[bookingbusiness](../resources/bookingbusiness.md)创建新的**bookingAppointment** 。</span><span class="sxs-lookup"><span data-stu-id="0e248-115">Create a new **bookingAppointment** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="0e248-116">获取 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="0e248-116">Get bookingAppointment</span></span>](../api/bookingappointment-get.md) | [<span data-ttu-id="0e248-117">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="0e248-117">bookingAppointment</span></span>](bookingappointment.md) |<span data-ttu-id="0e248-118">读取**bookingAppointment**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e248-118">Read the properties and relationships of **bookingAppointment** object.</span></span>|
|[<span data-ttu-id="0e248-119">更新</span><span class="sxs-lookup"><span data-stu-id="0e248-119">Update</span></span>](../api/bookingappointment-update.md) | [<span data-ttu-id="0e248-120">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="0e248-120">bookingAppointment</span></span>](bookingappointment.md)    |<span data-ttu-id="0e248-121">更新**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="0e248-121">Update a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="0e248-122">删除</span><span class="sxs-lookup"><span data-stu-id="0e248-122">Delete</span></span>](../api/bookingappointment-delete.md) | <span data-ttu-id="0e248-123">无</span><span class="sxs-lookup"><span data-stu-id="0e248-123">None</span></span> |<span data-ttu-id="0e248-124">删除**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="0e248-124">Delete a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="0e248-125">Cancel</span><span class="sxs-lookup"><span data-stu-id="0e248-125">Cancel</span></span>](../api/bookingappointment-cancel.md)|<span data-ttu-id="0e248-126">无</span><span class="sxs-lookup"><span data-stu-id="0e248-126">None</span></span>| <span data-ttu-id="0e248-127">取消**bookingAppointment**对象。</span><span class="sxs-lookup"><span data-stu-id="0e248-127">Cancel a **bookingAppointment** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e248-128">属性</span><span class="sxs-lookup"><span data-stu-id="0e248-128">Properties</span></span>
| <span data-ttu-id="0e248-129">属性</span><span class="sxs-lookup"><span data-stu-id="0e248-129">Property</span></span>     | <span data-ttu-id="0e248-130">类型</span><span class="sxs-lookup"><span data-stu-id="0e248-130">Type</span></span>   |<span data-ttu-id="0e248-131">说明</span><span class="sxs-lookup"><span data-stu-id="0e248-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e248-132">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0e248-132">customerEmailAddress</span></span>|<span data-ttu-id="0e248-133">String</span><span class="sxs-lookup"><span data-stu-id="0e248-133">String</span></span>|<span data-ttu-id="0e248-134">预订约会的[bookingCustomer](bookingcustomer.md)的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="0e248-134">The SMTP address of the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="0e248-135">customerId</span><span class="sxs-lookup"><span data-stu-id="0e248-135">customerId</span></span>|<span data-ttu-id="0e248-136">String</span><span class="sxs-lookup"><span data-stu-id="0e248-136">String</span></span>|<span data-ttu-id="0e248-137">此约会的[bookingCustomer](bookingcustomer.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="0e248-137">The ID of the [bookingCustomer](bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="0e248-138">如果创建约会时未指定 ID, 则会创建一个新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="0e248-138">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="0e248-139">设置后, 应考虑**customerId**不可变。</span><span class="sxs-lookup"><span data-stu-id="0e248-139">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="0e248-140">customerLocation</span><span class="sxs-lookup"><span data-stu-id="0e248-140">customerLocation</span></span>|[<span data-ttu-id="0e248-141">location</span><span class="sxs-lookup"><span data-stu-id="0e248-141">location</span></span>](location.md)|<span data-ttu-id="0e248-142">表示预订约会的[bookingCustomer](bookingcustomer.md)的位置信息。</span><span class="sxs-lookup"><span data-stu-id="0e248-142">Represents location information for the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="0e248-143">customerName</span><span class="sxs-lookup"><span data-stu-id="0e248-143">customerName</span></span>|<span data-ttu-id="0e248-144">String</span><span class="sxs-lookup"><span data-stu-id="0e248-144">String</span></span>|<span data-ttu-id="0e248-145">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="0e248-145">The customer's name.</span></span>|
|<span data-ttu-id="0e248-146">customerNotes</span><span class="sxs-lookup"><span data-stu-id="0e248-146">customerNotes</span></span>|<span data-ttu-id="0e248-147">String</span><span class="sxs-lookup"><span data-stu-id="0e248-147">String</span></span>|<span data-ttu-id="0e248-148">来自与此约会相关联的客户的注释。</span><span class="sxs-lookup"><span data-stu-id="0e248-148">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="0e248-149">仅当按 ID 读取此**bookingAppointment**时, 才能获取该值。</span><span class="sxs-lookup"><span data-stu-id="0e248-149">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="0e248-150">只有在最初创建新客户的约会时, 才能设置该属性。</span><span class="sxs-lookup"><span data-stu-id="0e248-150">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="0e248-151">然后, 将从**customerId**表示的客户计算该值。</span><span class="sxs-lookup"><span data-stu-id="0e248-151">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="0e248-152">customerPhone</span><span class="sxs-lookup"><span data-stu-id="0e248-152">customerPhone</span></span>|<span data-ttu-id="0e248-153">String</span><span class="sxs-lookup"><span data-stu-id="0e248-153">String</span></span>|<span data-ttu-id="0e248-154">客户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="0e248-154">The customer's phone number.</span></span>|
|<span data-ttu-id="0e248-155">duration</span><span class="sxs-lookup"><span data-stu-id="0e248-155">duration</span></span>|<span data-ttu-id="0e248-156">持续时间</span><span class="sxs-lookup"><span data-stu-id="0e248-156">Duration</span></span>|<span data-ttu-id="0e248-157">约会的长度, 以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="0e248-157">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="0e248-158">end</span><span class="sxs-lookup"><span data-stu-id="0e248-158">end</span></span>|[<span data-ttu-id="0e248-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0e248-159">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0e248-160">约会结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="0e248-160">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="0e248-161">id</span><span class="sxs-lookup"><span data-stu-id="0e248-161">id</span></span>|<span data-ttu-id="0e248-162">String</span><span class="sxs-lookup"><span data-stu-id="0e248-162">String</span></span>| <span data-ttu-id="0e248-163">**bookingAppointment**的 ID。</span><span class="sxs-lookup"><span data-stu-id="0e248-163">The ID of the **bookingAppointment**.</span></span> <span data-ttu-id="0e248-164">只读。</span><span class="sxs-lookup"><span data-stu-id="0e248-164">Read-only.</span></span>|
|<span data-ttu-id="0e248-165">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="0e248-165">invoiceAmount</span></span>|<span data-ttu-id="0e248-166">双精度</span><span class="sxs-lookup"><span data-stu-id="0e248-166">Double</span></span>|<span data-ttu-id="0e248-167">发票上的计费金额。</span><span class="sxs-lookup"><span data-stu-id="0e248-167">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="0e248-168">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="0e248-168">invoiceDate</span></span>|[<span data-ttu-id="0e248-169">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0e248-169">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0e248-170">此约会的发票的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="0e248-170">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="0e248-171">invoiceId</span><span class="sxs-lookup"><span data-stu-id="0e248-171">invoiceId</span></span>|<span data-ttu-id="0e248-172">String</span><span class="sxs-lookup"><span data-stu-id="0e248-172">String</span></span>|<span data-ttu-id="0e248-173">发票的 ID。</span><span class="sxs-lookup"><span data-stu-id="0e248-173">The ID of the invoice.</span></span>|
|<span data-ttu-id="0e248-174">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="0e248-174">invoiceStatus</span></span>|<span data-ttu-id="0e248-175">string</span><span class="sxs-lookup"><span data-stu-id="0e248-175">string</span></span>| <span data-ttu-id="0e248-176">发票的状态。</span><span class="sxs-lookup"><span data-stu-id="0e248-176">The status of the invoice.</span></span> <span data-ttu-id="0e248-177">可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="0e248-177">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="0e248-178">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="0e248-178">invoiceUrl</span></span>|<span data-ttu-id="0e248-179">String</span><span class="sxs-lookup"><span data-stu-id="0e248-179">String</span></span>|<span data-ttu-id="0e248-180">Microsoft 预订中发票的 URL。</span><span class="sxs-lookup"><span data-stu-id="0e248-180">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="0e248-181">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="0e248-181">optOutOfCustomerEmail</span></span>|<span data-ttu-id="0e248-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e248-182">Boolean</span></span>|<span data-ttu-id="0e248-183">如果为 True, 则表示此约会的[bookingCustomer](bookingcustomer.md)不希望收到此约会的确认。</span><span class="sxs-lookup"><span data-stu-id="0e248-183">True indicates that the [bookingCustomer](bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="0e248-184">postBuffer</span><span class="sxs-lookup"><span data-stu-id="0e248-184">postBuffer</span></span>|<span data-ttu-id="0e248-185">持续时间</span><span class="sxs-lookup"><span data-stu-id="0e248-185">Duration</span></span>|<span data-ttu-id="0e248-186">在约会结束后保留的时间长度, 例如, 进行清理。</span><span class="sxs-lookup"><span data-stu-id="0e248-186">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="0e248-187">值以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="0e248-187">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="0e248-188">preBuffer</span><span class="sxs-lookup"><span data-stu-id="0e248-188">preBuffer</span></span>|<span data-ttu-id="0e248-189">持续时间</span><span class="sxs-lookup"><span data-stu-id="0e248-189">Duration</span></span>|<span data-ttu-id="0e248-190">在约会开始之前保留的时间量 (以供准备) 为例。</span><span class="sxs-lookup"><span data-stu-id="0e248-190">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="0e248-191">值以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="0e248-191">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="0e248-192">特价</span><span class="sxs-lookup"><span data-stu-id="0e248-192">price</span></span>|<span data-ttu-id="0e248-193">双精度</span><span class="sxs-lookup"><span data-stu-id="0e248-193">Double</span></span>|<span data-ttu-id="0e248-194">指定[bookingService](bookingservice.md)的约会的常规价格。</span><span class="sxs-lookup"><span data-stu-id="0e248-194">The regular price for an appointment for the specified [bookingService](bookingservice.md).</span></span>|
|<span data-ttu-id="0e248-195">priceType</span><span class="sxs-lookup"><span data-stu-id="0e248-195">priceType</span></span>|<span data-ttu-id="0e248-196">string</span><span class="sxs-lookup"><span data-stu-id="0e248-196">string</span></span>| <span data-ttu-id="0e248-197">一种设置, 可为服务的定价结构提供灵活性。</span><span class="sxs-lookup"><span data-stu-id="0e248-197">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="0e248-198">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="0e248-198">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="0e248-199">提醒</span><span class="sxs-lookup"><span data-stu-id="0e248-199">reminders</span></span>|<span data-ttu-id="0e248-200">[bookingReminder](bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e248-200">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="0e248-201">为此约会发送的客户提醒的集合。</span><span class="sxs-lookup"><span data-stu-id="0e248-201">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="0e248-202">此属性的值仅在按 ID 读取此**bookingAppointment**时可用。</span><span class="sxs-lookup"><span data-stu-id="0e248-202">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="0e248-203">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="0e248-203">selfServiceAppointmentId</span></span>|<span data-ttu-id="0e248-204">String</span><span class="sxs-lookup"><span data-stu-id="0e248-204">String</span></span>|<span data-ttu-id="0e248-205">约会的其他跟踪 ID, 如果约会是由客户在日程安排页面上直接创建的, 而不是代表客户由教职员工成员创建的。</span><span class="sxs-lookup"><span data-stu-id="0e248-205">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="0e248-206">服务 Id</span><span class="sxs-lookup"><span data-stu-id="0e248-206">serviceId</span></span>|<span data-ttu-id="0e248-207">String</span><span class="sxs-lookup"><span data-stu-id="0e248-207">String</span></span>|<span data-ttu-id="0e248-208">与此约会相关联的[bookingService](bookingservice.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="0e248-208">The ID of the [bookingService](bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="0e248-209">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="0e248-209">serviceLocation</span></span>|[<span data-ttu-id="0e248-210">location</span><span class="sxs-lookup"><span data-stu-id="0e248-210">location</span></span>](location.md)|<span data-ttu-id="0e248-211">服务的传递位置。</span><span class="sxs-lookup"><span data-stu-id="0e248-211">The location where the service is delivered.</span></span>|
|<span data-ttu-id="0e248-212">serviceName</span><span class="sxs-lookup"><span data-stu-id="0e248-212">serviceName</span></span>|<span data-ttu-id="0e248-213">String</span><span class="sxs-lookup"><span data-stu-id="0e248-213">String</span></span>|<span data-ttu-id="0e248-214">与此约会相关联的**bookingService**的名称。</span><span class="sxs-lookup"><span data-stu-id="0e248-214">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="0e248-215">创建新约会时, 此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="0e248-215">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="0e248-216">如果未指定, 则通过**serviceId**属性从与约会关联的服务计算。</span><span class="sxs-lookup"><span data-stu-id="0e248-216">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="0e248-217">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="0e248-217">serviceNotes</span></span>|<span data-ttu-id="0e248-218">String</span><span class="sxs-lookup"><span data-stu-id="0e248-218">String</span></span>|<span data-ttu-id="0e248-219">来自[bookingStaffMember](bookingstaffmember.md)的注释。</span><span class="sxs-lookup"><span data-stu-id="0e248-219">Notes from a [bookingStaffMember](bookingstaffmember.md).</span></span> <span data-ttu-id="0e248-220">此属性的值仅在按 ID 读取此**bookingAppointment**时可用。</span><span class="sxs-lookup"><span data-stu-id="0e248-220">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="0e248-221">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="0e248-221">staffMemberIds</span></span>|<span data-ttu-id="0e248-222">String 集合</span><span class="sxs-lookup"><span data-stu-id="0e248-222">String collection</span></span>|<span data-ttu-id="0e248-223">在此约会中计划的每个[bookingStaffMember](bookingstaffmember.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="0e248-223">The ID of each [bookingStaffMember](bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="0e248-224">start</span><span class="sxs-lookup"><span data-stu-id="0e248-224">start</span></span>|[<span data-ttu-id="0e248-225">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0e248-225">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0e248-226">约会开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="0e248-226">The date, time, and time zone that the appointment begins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e248-227">关系</span><span class="sxs-lookup"><span data-stu-id="0e248-227">Relationships</span></span>
<span data-ttu-id="0e248-228">无</span><span class="sxs-lookup"><span data-stu-id="0e248-228">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0e248-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e248-229">JSON representation</span></span>

<span data-ttu-id="0e248-230">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e248-230">The following is a JSON representation of the resource.</span></span>

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
