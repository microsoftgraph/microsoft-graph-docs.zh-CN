---
title: 更新 bookingappointment
description: 更新指定 bookingbusiness 中的 bookingAppointment 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 3ba01a0fa6d1d28070471226a0c5f2ebae95006e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318416"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="01f56-103">更新 bookingappointment</span><span class="sxs-lookup"><span data-stu-id="01f56-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01f56-104">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingAppointment](../resources/bookingappointment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="01f56-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="01f56-105">权限</span><span class="sxs-lookup"><span data-stu-id="01f56-105">Permissions</span></span>
<span data-ttu-id="01f56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01f56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f56-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="01f56-108">Permission type</span></span>      | <span data-ttu-id="01f56-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01f56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01f56-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01f56-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="01f56-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 All</span><span class="sxs-lookup"><span data-stu-id="01f56-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="01f56-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01f56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f56-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="01f56-113">Not supported.</span></span>   |
|<span data-ttu-id="01f56-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="01f56-114">Application</span></span> | <span data-ttu-id="01f56-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01f56-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="01f56-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01f56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="01f56-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="01f56-117">Optional request headers</span></span>
| <span data-ttu-id="01f56-118">名称</span><span class="sxs-lookup"><span data-stu-id="01f56-118">Name</span></span>       | <span data-ttu-id="01f56-119">说明</span><span class="sxs-lookup"><span data-stu-id="01f56-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="01f56-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f56-120">Authorization</span></span>  | <span data-ttu-id="01f56-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="01f56-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="01f56-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="01f56-122">Request body</span></span>
<span data-ttu-id="01f56-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="01f56-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="01f56-126">属性</span><span class="sxs-lookup"><span data-stu-id="01f56-126">Property</span></span>     | <span data-ttu-id="01f56-127">类型</span><span class="sxs-lookup"><span data-stu-id="01f56-127">Type</span></span>   |<span data-ttu-id="01f56-128">说明</span><span class="sxs-lookup"><span data-stu-id="01f56-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01f56-129">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="01f56-129">customerEmailAddress</span></span>|<span data-ttu-id="01f56-130">String</span><span class="sxs-lookup"><span data-stu-id="01f56-130">String</span></span>|<span data-ttu-id="01f56-131">预订约会的[bookingCustomer](../resources/bookingcustomer.md)的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="01f56-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="01f56-132">customerId</span><span class="sxs-lookup"><span data-stu-id="01f56-132">customerId</span></span>|<span data-ttu-id="01f56-133">String</span><span class="sxs-lookup"><span data-stu-id="01f56-133">String</span></span>|<span data-ttu-id="01f56-134">此约会的[bookingCustomer](../resources/bookingcustomer.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="01f56-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="01f56-135">如果创建约会时未指定 ID, 则会创建一个新的**bookingCustomer**对象。</span><span class="sxs-lookup"><span data-stu-id="01f56-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="01f56-136">设置后, 应考虑**customerId**不可变。</span><span class="sxs-lookup"><span data-stu-id="01f56-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="01f56-137">customerLocation</span><span class="sxs-lookup"><span data-stu-id="01f56-137">customerLocation</span></span>|[<span data-ttu-id="01f56-138">location</span><span class="sxs-lookup"><span data-stu-id="01f56-138">location</span></span>](../resources/location.md)|<span data-ttu-id="01f56-139">表示预订约会的[bookingCustomer](../resources/bookingcustomer.md)的位置信息。</span><span class="sxs-lookup"><span data-stu-id="01f56-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="01f56-140">customerName</span><span class="sxs-lookup"><span data-stu-id="01f56-140">customerName</span></span>|<span data-ttu-id="01f56-141">String</span><span class="sxs-lookup"><span data-stu-id="01f56-141">String</span></span>|<span data-ttu-id="01f56-142">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="01f56-142">The customer's name.</span></span>|
|<span data-ttu-id="01f56-143">customerNotes</span><span class="sxs-lookup"><span data-stu-id="01f56-143">customerNotes</span></span>|<span data-ttu-id="01f56-144">String</span><span class="sxs-lookup"><span data-stu-id="01f56-144">String</span></span>|<span data-ttu-id="01f56-145">来自与此约会相关联的客户的注释。</span><span class="sxs-lookup"><span data-stu-id="01f56-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="01f56-146">仅当按 ID 读取此**bookingAppointment**时, 才能获取该值。</span><span class="sxs-lookup"><span data-stu-id="01f56-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="01f56-147">只有在最初创建新客户的约会时, 才能设置该属性。</span><span class="sxs-lookup"><span data-stu-id="01f56-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="01f56-148">然后, 将从**customerId**表示的客户计算该值。</span><span class="sxs-lookup"><span data-stu-id="01f56-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="01f56-149">customerPhone</span><span class="sxs-lookup"><span data-stu-id="01f56-149">customerPhone</span></span>|<span data-ttu-id="01f56-150">String</span><span class="sxs-lookup"><span data-stu-id="01f56-150">String</span></span>|<span data-ttu-id="01f56-151">客户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="01f56-151">The customer's phone number.</span></span>|
|<span data-ttu-id="01f56-152">duration</span><span class="sxs-lookup"><span data-stu-id="01f56-152">duration</span></span>|<span data-ttu-id="01f56-153">持续时间</span><span class="sxs-lookup"><span data-stu-id="01f56-153">Duration</span></span>|<span data-ttu-id="01f56-154">约会的长度, 以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="01f56-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="01f56-155">end</span><span class="sxs-lookup"><span data-stu-id="01f56-155">end</span></span>|[<span data-ttu-id="01f56-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="01f56-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="01f56-157">约会结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="01f56-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="01f56-158">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="01f56-158">invoiceAmount</span></span>|<span data-ttu-id="01f56-159">双精度</span><span class="sxs-lookup"><span data-stu-id="01f56-159">Double</span></span>|<span data-ttu-id="01f56-160">发票上的计费金额。</span><span class="sxs-lookup"><span data-stu-id="01f56-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="01f56-161">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="01f56-161">invoiceDate</span></span>|[<span data-ttu-id="01f56-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="01f56-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="01f56-163">此约会的发票的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="01f56-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="01f56-164">invoiceId</span><span class="sxs-lookup"><span data-stu-id="01f56-164">invoiceId</span></span>|<span data-ttu-id="01f56-165">String</span><span class="sxs-lookup"><span data-stu-id="01f56-165">String</span></span>|<span data-ttu-id="01f56-166">发票的 ID。</span><span class="sxs-lookup"><span data-stu-id="01f56-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="01f56-167">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="01f56-167">invoiceStatus</span></span>|<span data-ttu-id="01f56-168">string</span><span class="sxs-lookup"><span data-stu-id="01f56-168">string</span></span>| <span data-ttu-id="01f56-169">发票的状态。</span><span class="sxs-lookup"><span data-stu-id="01f56-169">The status of the invoice.</span></span> <span data-ttu-id="01f56-170">可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="01f56-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="01f56-171">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="01f56-171">invoiceUrl</span></span>|<span data-ttu-id="01f56-172">String</span><span class="sxs-lookup"><span data-stu-id="01f56-172">String</span></span>|<span data-ttu-id="01f56-173">Microsoft 预订中发票的 URL。</span><span class="sxs-lookup"><span data-stu-id="01f56-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="01f56-174">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="01f56-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="01f56-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="01f56-175">Boolean</span></span>|<span data-ttu-id="01f56-176">如果为 True, 则表示此约会的[bookingCustomer](../resources/bookingcustomer.md)不希望收到此约会的确认。</span><span class="sxs-lookup"><span data-stu-id="01f56-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="01f56-177">postBuffer</span><span class="sxs-lookup"><span data-stu-id="01f56-177">postBuffer</span></span>|<span data-ttu-id="01f56-178">持续时间</span><span class="sxs-lookup"><span data-stu-id="01f56-178">Duration</span></span>|<span data-ttu-id="01f56-179">在约会结束后保留的时间长度, 例如, 进行清理。</span><span class="sxs-lookup"><span data-stu-id="01f56-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="01f56-180">值以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="01f56-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="01f56-181">preBuffer</span><span class="sxs-lookup"><span data-stu-id="01f56-181">preBuffer</span></span>|<span data-ttu-id="01f56-182">持续时间</span><span class="sxs-lookup"><span data-stu-id="01f56-182">Duration</span></span>|<span data-ttu-id="01f56-183">在约会开始之前保留的时间量 (以供准备) 为例。</span><span class="sxs-lookup"><span data-stu-id="01f56-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="01f56-184">值以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="01f56-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="01f56-185">特价</span><span class="sxs-lookup"><span data-stu-id="01f56-185">price</span></span>|<span data-ttu-id="01f56-186">双精度</span><span class="sxs-lookup"><span data-stu-id="01f56-186">Double</span></span>|<span data-ttu-id="01f56-187">指定[bookingService](../resources/bookingservice.md)的约会的常规价格。</span><span class="sxs-lookup"><span data-stu-id="01f56-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="01f56-188">priceType</span><span class="sxs-lookup"><span data-stu-id="01f56-188">priceType</span></span>|<span data-ttu-id="01f56-189">string</span><span class="sxs-lookup"><span data-stu-id="01f56-189">string</span></span>| <span data-ttu-id="01f56-190">一种设置, 可为服务的定价结构提供灵活性。</span><span class="sxs-lookup"><span data-stu-id="01f56-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="01f56-191">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="01f56-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="01f56-192">提醒</span><span class="sxs-lookup"><span data-stu-id="01f56-192">reminders</span></span>|<span data-ttu-id="01f56-193">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="01f56-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="01f56-194">为此约会发送的客户提醒的集合。</span><span class="sxs-lookup"><span data-stu-id="01f56-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="01f56-195">此属性的值仅在按 ID 读取此**bookingAppointment**时可用。</span><span class="sxs-lookup"><span data-stu-id="01f56-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="01f56-196">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="01f56-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="01f56-197">String</span><span class="sxs-lookup"><span data-stu-id="01f56-197">String</span></span>|<span data-ttu-id="01f56-198">约会的其他跟踪 ID, 如果约会是由客户在日程安排页面上直接创建的, 而不是代表客户由教职员工成员创建的。</span><span class="sxs-lookup"><span data-stu-id="01f56-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="01f56-199">服务 Id</span><span class="sxs-lookup"><span data-stu-id="01f56-199">serviceId</span></span>|<span data-ttu-id="01f56-200">String</span><span class="sxs-lookup"><span data-stu-id="01f56-200">String</span></span>|<span data-ttu-id="01f56-201">与此约会相关联的[bookingService](../resources/bookingservice.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="01f56-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="01f56-202">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="01f56-202">serviceLocation</span></span>|[<span data-ttu-id="01f56-203">location</span><span class="sxs-lookup"><span data-stu-id="01f56-203">location</span></span>](../resources/location.md)|<span data-ttu-id="01f56-204">服务的传递位置。</span><span class="sxs-lookup"><span data-stu-id="01f56-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="01f56-205">serviceName</span><span class="sxs-lookup"><span data-stu-id="01f56-205">serviceName</span></span>|<span data-ttu-id="01f56-206">String</span><span class="sxs-lookup"><span data-stu-id="01f56-206">String</span></span>|<span data-ttu-id="01f56-207">与此约会相关联的**bookingService**的名称。</span><span class="sxs-lookup"><span data-stu-id="01f56-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="01f56-208">创建新约会时, 此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="01f56-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="01f56-209">如果未指定, 则通过**serviceId**属性从与约会关联的服务计算。</span><span class="sxs-lookup"><span data-stu-id="01f56-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="01f56-210">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="01f56-210">serviceNotes</span></span>|<span data-ttu-id="01f56-211">String</span><span class="sxs-lookup"><span data-stu-id="01f56-211">String</span></span>|<span data-ttu-id="01f56-212">来自[bookingStaffMember](../resources/bookingstaffmember.md)的注释。</span><span class="sxs-lookup"><span data-stu-id="01f56-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="01f56-213">此属性的值仅在按 ID 读取此**bookingAppointment**时可用。</span><span class="sxs-lookup"><span data-stu-id="01f56-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="01f56-214">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="01f56-214">staffMemberIds</span></span>|<span data-ttu-id="01f56-215">String collection</span><span class="sxs-lookup"><span data-stu-id="01f56-215">String collection</span></span>|<span data-ttu-id="01f56-216">在此约会中计划的每个[bookingStaffMember](../resources/bookingstaffmember.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="01f56-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="01f56-217">start</span><span class="sxs-lookup"><span data-stu-id="01f56-217">start</span></span>|[<span data-ttu-id="01f56-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="01f56-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="01f56-219">约会开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="01f56-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="01f56-220">响应</span><span class="sxs-lookup"><span data-stu-id="01f56-220">Response</span></span>
<span data-ttu-id="01f56-p113">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="01f56-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01f56-223">示例</span><span class="sxs-lookup"><span data-stu-id="01f56-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01f56-224">请求</span><span class="sxs-lookup"><span data-stu-id="01f56-224">Request</span></span>
<span data-ttu-id="01f56-225">下面的示例将服务日期更改为一天, 并同时更新发票日期。</span><span class="sxs-lookup"><span data-stu-id="01f56-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01f56-226">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="01f56-226">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="01f56-227">C#</span><span class="sxs-lookup"><span data-stu-id="01f56-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01f56-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01f56-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01f56-229">目标-C</span><span class="sxs-lookup"><span data-stu-id="01f56-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="01f56-230">Java</span><span class="sxs-lookup"><span data-stu-id="01f56-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01f56-231">响应</span><span class="sxs-lookup"><span data-stu-id="01f56-231">Response</span></span>
<span data-ttu-id="01f56-232">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01f56-232">The following is an example of the response.</span></span>
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
  ]
}
-->
