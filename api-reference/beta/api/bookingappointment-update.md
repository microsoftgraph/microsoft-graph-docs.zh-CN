---
title: 更新 bookingappointment
description: 更新中指定 bookingbusiness bookingAppointment 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cde8a309e3544f5ed5cdf84f7c50d33e95084526
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529234"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="3cad2-103">更新 bookingappointment</span><span class="sxs-lookup"><span data-stu-id="3cad2-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cad2-104">更新中指定[bookingbusiness](../resources/bookingbusiness.md) [bookingAppointment](../resources/bookingappointment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3cad2-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3cad2-105">权限</span><span class="sxs-lookup"><span data-stu-id="3cad2-105">Permissions</span></span>
<span data-ttu-id="3cad2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cad2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cad2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cad2-108">Permission type</span></span>      | <span data-ttu-id="3cad2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cad2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cad2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cad2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3cad2-111">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3cad2-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3cad2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cad2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cad2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cad2-113">Not supported.</span></span>   |
|<span data-ttu-id="3cad2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cad2-114">Application</span></span> | <span data-ttu-id="3cad2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cad2-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3cad2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cad2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3cad2-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="3cad2-117">Optional request headers</span></span>
| <span data-ttu-id="3cad2-118">名称</span><span class="sxs-lookup"><span data-stu-id="3cad2-118">Name</span></span>       | <span data-ttu-id="3cad2-119">说明</span><span class="sxs-lookup"><span data-stu-id="3cad2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3cad2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cad2-120">Authorization</span></span>  | <span data-ttu-id="3cad2-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3cad2-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cad2-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cad2-122">Request body</span></span>
<span data-ttu-id="3cad2-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3cad2-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3cad2-126">属性</span><span class="sxs-lookup"><span data-stu-id="3cad2-126">Property</span></span>     | <span data-ttu-id="3cad2-127">类型</span><span class="sxs-lookup"><span data-stu-id="3cad2-127">Type</span></span>   |<span data-ttu-id="3cad2-128">说明</span><span class="sxs-lookup"><span data-stu-id="3cad2-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cad2-129">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3cad2-129">customerEmailAddress</span></span>|<span data-ttu-id="3cad2-130">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-130">String</span></span>|<span data-ttu-id="3cad2-131">预订约会[bookingCustomer](../resources/bookingcustomer.md) SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="3cad2-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="3cad2-132">customerId</span><span class="sxs-lookup"><span data-stu-id="3cad2-132">customerId</span></span>|<span data-ttu-id="3cad2-133">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-133">String</span></span>|<span data-ttu-id="3cad2-134">该约会的[bookingCustomer](../resources/bookingcustomer.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="3cad2-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="3cad2-135">如果未指定 ID 创建约会时，将创建一个新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="3cad2-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="3cad2-136">设置后，您应考虑**customerId**变。</span><span class="sxs-lookup"><span data-stu-id="3cad2-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="3cad2-137">customerLocation</span><span class="sxs-lookup"><span data-stu-id="3cad2-137">customerLocation</span></span>|[<span data-ttu-id="3cad2-138">location</span><span class="sxs-lookup"><span data-stu-id="3cad2-138">location</span></span>](../resources/location.md)|<span data-ttu-id="3cad2-139">代表[bookingCustomer](../resources/bookingcustomer.md)预订约会的位置信息。</span><span class="sxs-lookup"><span data-stu-id="3cad2-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="3cad2-140">customerName</span><span class="sxs-lookup"><span data-stu-id="3cad2-140">customerName</span></span>|<span data-ttu-id="3cad2-141">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-141">String</span></span>|<span data-ttu-id="3cad2-142">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="3cad2-142">The customer's name.</span></span>|
|<span data-ttu-id="3cad2-143">customerNotes</span><span class="sxs-lookup"><span data-stu-id="3cad2-143">customerNotes</span></span>|<span data-ttu-id="3cad2-144">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-144">String</span></span>|<span data-ttu-id="3cad2-145">从与此约会关联的客户的备注。</span><span class="sxs-lookup"><span data-stu-id="3cad2-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="3cad2-146">您可以获取仅当读取此**bookingAppointment**其 id 值</span><span class="sxs-lookup"><span data-stu-id="3cad2-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="3cad2-147">仅在最初使用新的客户创建约会时，您可以设置该属性。</span><span class="sxs-lookup"><span data-stu-id="3cad2-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="3cad2-148">此时，从由**customerId**客户计算的值。</span><span class="sxs-lookup"><span data-stu-id="3cad2-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="3cad2-149">customerPhone</span><span class="sxs-lookup"><span data-stu-id="3cad2-149">customerPhone</span></span>|<span data-ttu-id="3cad2-150">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-150">String</span></span>|<span data-ttu-id="3cad2-151">客户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="3cad2-151">The customer's phone number.</span></span>|
|<span data-ttu-id="3cad2-152">duration</span><span class="sxs-lookup"><span data-stu-id="3cad2-152">duration</span></span>|<span data-ttu-id="3cad2-153">持续时间</span><span class="sxs-lookup"><span data-stu-id="3cad2-153">Duration</span></span>|<span data-ttu-id="3cad2-154">约会中[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式的长度。</span><span class="sxs-lookup"><span data-stu-id="3cad2-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="3cad2-155">end</span><span class="sxs-lookup"><span data-stu-id="3cad2-155">end</span></span>|[<span data-ttu-id="3cad2-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3cad2-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3cad2-157">日期、 时间和约会的结束的时区。</span><span class="sxs-lookup"><span data-stu-id="3cad2-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="3cad2-158">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="3cad2-158">invoiceAmount</span></span>|<span data-ttu-id="3cad2-159">双精度</span><span class="sxs-lookup"><span data-stu-id="3cad2-159">Double</span></span>|<span data-ttu-id="3cad2-160">记帐的发票量。</span><span class="sxs-lookup"><span data-stu-id="3cad2-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="3cad2-161">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="3cad2-161">invoiceDate</span></span>|[<span data-ttu-id="3cad2-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3cad2-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3cad2-163">日期、 时间和此约会的发票的时区。</span><span class="sxs-lookup"><span data-stu-id="3cad2-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="3cad2-164">invoiceId</span><span class="sxs-lookup"><span data-stu-id="3cad2-164">invoiceId</span></span>|<span data-ttu-id="3cad2-165">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-165">String</span></span>|<span data-ttu-id="3cad2-166">发票的 ID。</span><span class="sxs-lookup"><span data-stu-id="3cad2-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="3cad2-167">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="3cad2-167">invoiceStatus</span></span>|<span data-ttu-id="3cad2-168">string</span><span class="sxs-lookup"><span data-stu-id="3cad2-168">string</span></span>| <span data-ttu-id="3cad2-169">发票的状态。</span><span class="sxs-lookup"><span data-stu-id="3cad2-169">The status of the invoice.</span></span> <span data-ttu-id="3cad2-170">可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="3cad2-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="3cad2-171">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="3cad2-171">invoiceUrl</span></span>|<span data-ttu-id="3cad2-172">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-172">String</span></span>|<span data-ttu-id="3cad2-173">在 Microsoft 预订发票的 URL。</span><span class="sxs-lookup"><span data-stu-id="3cad2-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="3cad2-174">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="3cad2-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="3cad2-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cad2-175">Boolean</span></span>|<span data-ttu-id="3cad2-176">True 表示该约会的[bookingCustomer](../resources/bookingcustomer.md)不希望接收该约会的确认。</span><span class="sxs-lookup"><span data-stu-id="3cad2-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="3cad2-177">后</span><span class="sxs-lookup"><span data-stu-id="3cad2-177">postBuffer</span></span>|<span data-ttu-id="3cad2-178">持续时间</span><span class="sxs-lookup"><span data-stu-id="3cad2-178">Duration</span></span>|<span data-ttu-id="3cad2-179">保留后的清理，例如约会结束的时间量。</span><span class="sxs-lookup"><span data-stu-id="3cad2-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="3cad2-180">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。</span><span class="sxs-lookup"><span data-stu-id="3cad2-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="3cad2-181">缓冲区</span><span class="sxs-lookup"><span data-stu-id="3cad2-181">preBuffer</span></span>|<span data-ttu-id="3cad2-182">持续时间</span><span class="sxs-lookup"><span data-stu-id="3cad2-182">Duration</span></span>|<span data-ttu-id="3cad2-183">保留之前的准备，例如约会开始的时间量。</span><span class="sxs-lookup"><span data-stu-id="3cad2-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="3cad2-184">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。</span><span class="sxs-lookup"><span data-stu-id="3cad2-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="3cad2-185">Price</span><span class="sxs-lookup"><span data-stu-id="3cad2-185">price</span></span>|<span data-ttu-id="3cad2-186">双精度</span><span class="sxs-lookup"><span data-stu-id="3cad2-186">Double</span></span>|<span data-ttu-id="3cad2-187">指定[bookingService](../resources/bookingservice.md)约会正则价格。</span><span class="sxs-lookup"><span data-stu-id="3cad2-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="3cad2-188">priceType</span><span class="sxs-lookup"><span data-stu-id="3cad2-188">priceType</span></span>|<span data-ttu-id="3cad2-189">string</span><span class="sxs-lookup"><span data-stu-id="3cad2-189">string</span></span>| <span data-ttu-id="3cad2-190">为服务定价结构提供灵活性设置。</span><span class="sxs-lookup"><span data-stu-id="3cad2-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="3cad2-191">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="3cad2-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="3cad2-192">提醒</span><span class="sxs-lookup"><span data-stu-id="3cad2-192">reminders</span></span>|<span data-ttu-id="3cad2-193">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="3cad2-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="3cad2-194">客户提醒发送该约会的集合。</span><span class="sxs-lookup"><span data-stu-id="3cad2-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="3cad2-195">此属性的值时，可仅读取此**bookingAppointment**由其 id。</span><span class="sxs-lookup"><span data-stu-id="3cad2-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="3cad2-196">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="3cad2-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="3cad2-197">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-197">String</span></span>|<span data-ttu-id="3cad2-198">约会，如果约会的已创建直接通过计划页上的客户而不是由员工成员客户替的其他跟踪 ID。</span><span class="sxs-lookup"><span data-stu-id="3cad2-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="3cad2-199">服务 Id</span><span class="sxs-lookup"><span data-stu-id="3cad2-199">serviceId</span></span>|<span data-ttu-id="3cad2-200">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-200">String</span></span>|<span data-ttu-id="3cad2-201">与此约会相关联的[bookingService](../resources/bookingservice.md) ID。</span><span class="sxs-lookup"><span data-stu-id="3cad2-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="3cad2-202">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="3cad2-202">serviceLocation</span></span>|[<span data-ttu-id="3cad2-203">location</span><span class="sxs-lookup"><span data-stu-id="3cad2-203">location</span></span>](../resources/location.md)|<span data-ttu-id="3cad2-204">传递服务的位置的位置。</span><span class="sxs-lookup"><span data-stu-id="3cad2-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="3cad2-205">service_name</span><span class="sxs-lookup"><span data-stu-id="3cad2-205">serviceName</span></span>|<span data-ttu-id="3cad2-206">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-206">String</span></span>|<span data-ttu-id="3cad2-207">与此约会关联**bookingService**的名称。</span><span class="sxs-lookup"><span data-stu-id="3cad2-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="3cad2-208">创建一个新的约会时，此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="3cad2-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="3cad2-209">如果未指定，它是从与约会**serviceId**属性关联的服务进行计算。</span><span class="sxs-lookup"><span data-stu-id="3cad2-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="3cad2-210">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="3cad2-210">serviceNotes</span></span>|<span data-ttu-id="3cad2-211">String</span><span class="sxs-lookup"><span data-stu-id="3cad2-211">String</span></span>|<span data-ttu-id="3cad2-212">从[bookingStaffMember](../resources/bookingstaffmember.md)备注。</span><span class="sxs-lookup"><span data-stu-id="3cad2-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="3cad2-213">此属性的值时，可仅读取此**bookingAppointment**由其 id。</span><span class="sxs-lookup"><span data-stu-id="3cad2-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="3cad2-214">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="3cad2-214">staffMemberIds</span></span>|<span data-ttu-id="3cad2-215">String 集合</span><span class="sxs-lookup"><span data-stu-id="3cad2-215">String collection</span></span>|<span data-ttu-id="3cad2-216">每个[bookingStaffMember](../resources/bookingstaffmember.md)此约会中安排的 ID。</span><span class="sxs-lookup"><span data-stu-id="3cad2-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="3cad2-217">start</span><span class="sxs-lookup"><span data-stu-id="3cad2-217">start</span></span>|[<span data-ttu-id="3cad2-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3cad2-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3cad2-219">日期、 时间和时区约会的开始。</span><span class="sxs-lookup"><span data-stu-id="3cad2-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="3cad2-220">响应</span><span class="sxs-lookup"><span data-stu-id="3cad2-220">Response</span></span>
<span data-ttu-id="3cad2-p113">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3cad2-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3cad2-223">示例</span><span class="sxs-lookup"><span data-stu-id="3cad2-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cad2-224">请求</span><span class="sxs-lookup"><span data-stu-id="3cad2-224">Request</span></span>
<span data-ttu-id="3cad2-225">以下示例更改服务通过一天的日期和更新的发票日期。</span><span class="sxs-lookup"><span data-stu-id="3cad2-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3cad2-226">响应</span><span class="sxs-lookup"><span data-stu-id="3cad2-226">Response</span></span>
<span data-ttu-id="3cad2-227">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3cad2-227">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
