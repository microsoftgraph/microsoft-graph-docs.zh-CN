---
title: 更新 bookingappointment
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: fd63d11bf7a33751b6a271c57d0f871b5e6d474f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044006"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="80558-104">更新 bookingappointment</span><span class="sxs-lookup"><span data-stu-id="80558-104">Update bookingappointment</span></span>

 > <span data-ttu-id="80558-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="80558-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80558-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80558-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="80558-107">更新中指定[bookingbusiness](../resources/bookingbusiness.md) [bookingAppointment](../resources/bookingappointment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80558-107">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="80558-108">权限</span><span class="sxs-lookup"><span data-stu-id="80558-108">Permissions</span></span>
<span data-ttu-id="80558-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80558-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80558-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="80558-111">Permission type</span></span>      | <span data-ttu-id="80558-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80558-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80558-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80558-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="80558-114">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="80558-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="80558-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80558-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80558-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80558-116">Not supported.</span></span>   |
|<span data-ttu-id="80558-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="80558-117">Application</span></span> | <span data-ttu-id="80558-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="80558-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="80558-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80558-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="80558-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="80558-120">Optional request headers</span></span>
| <span data-ttu-id="80558-121">名称</span><span class="sxs-lookup"><span data-stu-id="80558-121">Name</span></span>       | <span data-ttu-id="80558-122">说明</span><span class="sxs-lookup"><span data-stu-id="80558-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="80558-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80558-123">Authorization</span></span>  | <span data-ttu-id="80558-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="80558-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="80558-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="80558-125">Request body</span></span>
<span data-ttu-id="80558-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="80558-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="80558-129">属性</span><span class="sxs-lookup"><span data-stu-id="80558-129">Property</span></span>     | <span data-ttu-id="80558-130">类型</span><span class="sxs-lookup"><span data-stu-id="80558-130">Type</span></span>   |<span data-ttu-id="80558-131">说明</span><span class="sxs-lookup"><span data-stu-id="80558-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80558-132">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="80558-132">customerEmailAddress</span></span>|<span data-ttu-id="80558-133">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-133">String</span></span>|<span data-ttu-id="80558-134">预订约会[bookingCustomer](../resources/bookingcustomer.md) SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="80558-134">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="80558-135">customerId</span><span class="sxs-lookup"><span data-stu-id="80558-135">customerId</span></span>|<span data-ttu-id="80558-136">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-136">String</span></span>|<span data-ttu-id="80558-137">该约会的[bookingCustomer](../resources/bookingcustomer.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="80558-137">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="80558-138">如果未指定 ID 创建约会时，将创建一个新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="80558-138">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="80558-139">设置后，您应考虑**customerId**变。</span><span class="sxs-lookup"><span data-stu-id="80558-139">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="80558-140">customerLocation</span><span class="sxs-lookup"><span data-stu-id="80558-140">customerLocation</span></span>|[<span data-ttu-id="80558-141">location</span><span class="sxs-lookup"><span data-stu-id="80558-141">location</span></span>](../resources/location.md)|<span data-ttu-id="80558-142">代表[bookingCustomer](../resources/bookingcustomer.md)预订约会的位置信息。</span><span class="sxs-lookup"><span data-stu-id="80558-142">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="80558-143">customerName</span><span class="sxs-lookup"><span data-stu-id="80558-143">customerName</span></span>|<span data-ttu-id="80558-144">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-144">String</span></span>|<span data-ttu-id="80558-145">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="80558-145">The customer's name.</span></span>|
|<span data-ttu-id="80558-146">customerNotes</span><span class="sxs-lookup"><span data-stu-id="80558-146">customerNotes</span></span>|<span data-ttu-id="80558-147">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-147">String</span></span>|<span data-ttu-id="80558-148">从与此约会关联的客户的备注。</span><span class="sxs-lookup"><span data-stu-id="80558-148">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="80558-149">您可以获取仅当读取此**bookingAppointment**其 id 值</span><span class="sxs-lookup"><span data-stu-id="80558-149">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="80558-150">仅在最初使用新的客户创建约会时，您可以设置该属性。</span><span class="sxs-lookup"><span data-stu-id="80558-150">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="80558-151">此时，从由**customerId**客户计算的值。</span><span class="sxs-lookup"><span data-stu-id="80558-151">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="80558-152">customerPhone</span><span class="sxs-lookup"><span data-stu-id="80558-152">customerPhone</span></span>|<span data-ttu-id="80558-153">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-153">String</span></span>|<span data-ttu-id="80558-154">客户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="80558-154">The customer's phone number.</span></span>|
|<span data-ttu-id="80558-155">duration</span><span class="sxs-lookup"><span data-stu-id="80558-155">duration</span></span>|<span data-ttu-id="80558-156">Duration</span><span class="sxs-lookup"><span data-stu-id="80558-156">Duration</span></span>|<span data-ttu-id="80558-157">约会中[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式的长度。</span><span class="sxs-lookup"><span data-stu-id="80558-157">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="80558-158">end</span><span class="sxs-lookup"><span data-stu-id="80558-158">end</span></span>|[<span data-ttu-id="80558-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="80558-159">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="80558-160">日期、 时间和约会的结束的时区。</span><span class="sxs-lookup"><span data-stu-id="80558-160">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="80558-161">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="80558-161">invoiceAmount</span></span>|<span data-ttu-id="80558-162">双精度数</span><span class="sxs-lookup"><span data-stu-id="80558-162">Double</span></span>|<span data-ttu-id="80558-163">记帐的发票量。</span><span class="sxs-lookup"><span data-stu-id="80558-163">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="80558-164">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="80558-164">invoiceDate</span></span>|[<span data-ttu-id="80558-165">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="80558-165">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="80558-166">日期、 时间和此约会的发票的时区。</span><span class="sxs-lookup"><span data-stu-id="80558-166">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="80558-167">invoiceId</span><span class="sxs-lookup"><span data-stu-id="80558-167">invoiceId</span></span>|<span data-ttu-id="80558-168">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-168">String</span></span>|<span data-ttu-id="80558-169">发票的 ID。</span><span class="sxs-lookup"><span data-stu-id="80558-169">The ID of the invoice.</span></span>|
|<span data-ttu-id="80558-170">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="80558-170">invoiceStatus</span></span>|<span data-ttu-id="80558-171">string</span><span class="sxs-lookup"><span data-stu-id="80558-171">string</span></span>| <span data-ttu-id="80558-172">发票的状态。</span><span class="sxs-lookup"><span data-stu-id="80558-172">The status of the invoice.</span></span> <span data-ttu-id="80558-173">可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="80558-173">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="80558-174">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="80558-174">invoiceUrl</span></span>|<span data-ttu-id="80558-175">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-175">String</span></span>|<span data-ttu-id="80558-176">在 Microsoft 预订发票的 URL。</span><span class="sxs-lookup"><span data-stu-id="80558-176">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="80558-177">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="80558-177">optOutOfCustomerEmail</span></span>|<span data-ttu-id="80558-178">布尔</span><span class="sxs-lookup"><span data-stu-id="80558-178">Boolean</span></span>|<span data-ttu-id="80558-179">True 表示该约会的[bookingCustomer](../resources/bookingcustomer.md)不希望接收该约会的确认。</span><span class="sxs-lookup"><span data-stu-id="80558-179">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="80558-180">后</span><span class="sxs-lookup"><span data-stu-id="80558-180">postBuffer</span></span>|<span data-ttu-id="80558-181">Duration</span><span class="sxs-lookup"><span data-stu-id="80558-181">Duration</span></span>|<span data-ttu-id="80558-182">保留后的清理，例如约会结束的时间量。</span><span class="sxs-lookup"><span data-stu-id="80558-182">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="80558-183">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。</span><span class="sxs-lookup"><span data-stu-id="80558-183">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="80558-184">缓冲区</span><span class="sxs-lookup"><span data-stu-id="80558-184">preBuffer</span></span>|<span data-ttu-id="80558-185">Duration</span><span class="sxs-lookup"><span data-stu-id="80558-185">Duration</span></span>|<span data-ttu-id="80558-186">保留之前的准备，例如约会开始的时间量。</span><span class="sxs-lookup"><span data-stu-id="80558-186">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="80558-187">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。</span><span class="sxs-lookup"><span data-stu-id="80558-187">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="80558-188">价格</span><span class="sxs-lookup"><span data-stu-id="80558-188">price</span></span>|<span data-ttu-id="80558-189">双精度数</span><span class="sxs-lookup"><span data-stu-id="80558-189">Double</span></span>|<span data-ttu-id="80558-190">指定[bookingService](../resources/bookingservice.md)约会正则价格。</span><span class="sxs-lookup"><span data-stu-id="80558-190">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="80558-191">priceType</span><span class="sxs-lookup"><span data-stu-id="80558-191">priceType</span></span>|<span data-ttu-id="80558-192">string</span><span class="sxs-lookup"><span data-stu-id="80558-192">string</span></span>| <span data-ttu-id="80558-193">为服务定价结构提供灵活性设置。</span><span class="sxs-lookup"><span data-stu-id="80558-193">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="80558-194">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="80558-194">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="80558-195">提醒</span><span class="sxs-lookup"><span data-stu-id="80558-195">reminders</span></span>|<span data-ttu-id="80558-196">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="80558-196">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="80558-197">客户提醒发送该约会的集合。</span><span class="sxs-lookup"><span data-stu-id="80558-197">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="80558-198">此属性的值时，可仅读取此**bookingAppointment**由其 id。</span><span class="sxs-lookup"><span data-stu-id="80558-198">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="80558-199">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="80558-199">selfServiceAppointmentId</span></span>|<span data-ttu-id="80558-200">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-200">String</span></span>|<span data-ttu-id="80558-201">约会，如果约会的已创建直接通过计划页上的客户而不是由员工成员客户替的其他跟踪 ID。</span><span class="sxs-lookup"><span data-stu-id="80558-201">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="80558-202">服务 Id</span><span class="sxs-lookup"><span data-stu-id="80558-202">serviceId</span></span>|<span data-ttu-id="80558-203">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-203">String</span></span>|<span data-ttu-id="80558-204">与此约会相关联的[bookingService](../resources/bookingservice.md) ID。</span><span class="sxs-lookup"><span data-stu-id="80558-204">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="80558-205">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="80558-205">serviceLocation</span></span>|[<span data-ttu-id="80558-206">location</span><span class="sxs-lookup"><span data-stu-id="80558-206">location</span></span>](../resources/location.md)|<span data-ttu-id="80558-207">传递服务的位置的位置。</span><span class="sxs-lookup"><span data-stu-id="80558-207">The location where the service is delivered.</span></span>|
|<span data-ttu-id="80558-208">serviceName</span><span class="sxs-lookup"><span data-stu-id="80558-208">serviceName</span></span>|<span data-ttu-id="80558-209">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-209">String</span></span>|<span data-ttu-id="80558-210">与此约会关联**bookingService**的名称。</span><span class="sxs-lookup"><span data-stu-id="80558-210">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="80558-211">创建一个新的约会时，此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="80558-211">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="80558-212">如果未指定，它是从与约会**serviceId**属性关联的服务进行计算。</span><span class="sxs-lookup"><span data-stu-id="80558-212">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="80558-213">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="80558-213">serviceNotes</span></span>|<span data-ttu-id="80558-214">字符串</span><span class="sxs-lookup"><span data-stu-id="80558-214">String</span></span>|<span data-ttu-id="80558-215">从[bookingStaffMember](../resources/bookingstaffmember.md)备注。</span><span class="sxs-lookup"><span data-stu-id="80558-215">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="80558-216">此属性的值时，可仅读取此**bookingAppointment**由其 id。</span><span class="sxs-lookup"><span data-stu-id="80558-216">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="80558-217">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="80558-217">staffMemberIds</span></span>|<span data-ttu-id="80558-218">String 集合</span><span class="sxs-lookup"><span data-stu-id="80558-218">String collection</span></span>|<span data-ttu-id="80558-219">每个[bookingStaffMember](../resources/bookingstaffmember.md)此约会中安排的 ID。</span><span class="sxs-lookup"><span data-stu-id="80558-219">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="80558-220">start</span><span class="sxs-lookup"><span data-stu-id="80558-220">start</span></span>|[<span data-ttu-id="80558-221">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="80558-221">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="80558-222">日期、 时间和时区约会的开始。</span><span class="sxs-lookup"><span data-stu-id="80558-222">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="80558-223">响应</span><span class="sxs-lookup"><span data-stu-id="80558-223">Response</span></span>
<span data-ttu-id="80558-p115">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="80558-p115">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80558-226">示例</span><span class="sxs-lookup"><span data-stu-id="80558-226">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80558-227">请求</span><span class="sxs-lookup"><span data-stu-id="80558-227">Request</span></span>
<span data-ttu-id="80558-228">以下示例更改服务通过一天的日期和更新的发票日期。</span><span class="sxs-lookup"><span data-stu-id="80558-228">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
##### <a name="response"></a><span data-ttu-id="80558-229">响应</span><span class="sxs-lookup"><span data-stu-id="80558-229">Response</span></span>
<span data-ttu-id="80558-230">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80558-230">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->