---
title: 使用 Microsoft Graph 中的 Microsoft Bookings API
description: Microsoft Bookings 可让企业组织和小型企业所有者以最少量的设置管理客户预订和信息。
localization_priority: Priority
author: arvindmicrosoft
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: c21cb95d140fa41711264ec0e6c71b7828b5a709
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118656"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="4cd75-103">使用 Microsoft Graph 中的 Microsoft Bookings API</span><span class="sxs-lookup"><span data-stu-id="4cd75-103">Use the Microsoft Bookings API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="4cd75-104">Microsoft Bookings 可让企业组织和小型企业所有者以最少量的设置管理客户预订和信息。</span><span class="sxs-lookup"><span data-stu-id="4cd75-104">Microsoft Bookings lets enterprise organization and small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="4cd75-105">企业所有者可以创建一个或多个企业，每个企业都提供一组服务。</span><span class="sxs-lookup"><span data-stu-id="4cd75-105">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="4cd75-106">所有者可以设置员工，并指定每名员工执行的服务。</span><span class="sxs-lookup"><span data-stu-id="4cd75-106">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="4cd75-107">客户可以通过在线或移动应用预约该企业中的特定服务。</span><span class="sxs-lookup"><span data-stu-id="4cd75-107">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="4cd75-108">Bookings 可确保为企业、员工和相关客户保持最新的约会时间。</span><span class="sxs-lookup"><span data-stu-id="4cd75-108">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="4cd75-109">就编程而言，Bookings API 中的 [bookingBusiness](bookingbusiness.md) 涉及以下对象：</span><span class="sxs-lookup"><span data-stu-id="4cd75-109">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="4cd75-110">一个或多个 [bookingStaffMember](bookingstaffmember.md) 对象</span><span class="sxs-lookup"><span data-stu-id="4cd75-110">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="4cd75-111">一个或多个 [bookingService](bookingservice.md) 对象</span><span class="sxs-lookup"><span data-stu-id="4cd75-111">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="4cd75-112">一组 [bookingAppointment](bookingappointment.md) 实例</span><span class="sxs-lookup"><span data-stu-id="4cd75-112">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="4cd75-113">一组 [bookingCustomer](bookingcustomer.md) 对象</span><span class="sxs-lookup"><span data-stu-id="4cd75-113">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="4cd75-114">使用 Bookings REST API</span><span class="sxs-lookup"><span data-stu-id="4cd75-114">Using the Bookings REST API</span></span>

<span data-ttu-id="4cd75-115">第一次客户预约之前，请完成以下步骤。</span><span class="sxs-lookup"><span data-stu-id="4cd75-115">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="4cd75-116">确保为相应的操作提供适当的[访问令牌](/graph/auth-overview)。</span><span class="sxs-lookup"><span data-stu-id="4cd75-116">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="4cd75-117">确保企业具有 [Microsoft 365 商业高级版](https://products.office.com/zh-CN/business/office-365-business-premium)订阅。</span><span class="sxs-lookup"><span data-stu-id="4cd75-117">Make sure the business has an [Microsoft 365 Business Premium](https://products.office.com/zh-CN/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="4cd75-118">通过向实体集发送 POST 操作来创建新的 **bookingBusiness**。</span><span class="sxs-lookup"><span data-stu-id="4cd75-118">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="4cd75-119">至少应为新企业指定客户将看到的名称：</span><span class="sxs-lookup"><span data-stu-id="4cd75-119">At minimum, you should specify a name for the new business that customers will see:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="4cd75-120">使用 POST 响应中返回的新 **bookingBusiness** 的 **id** 属性继续 [自定义](../api/bookingbusiness-update.md)企业设置，并为企业添加员工和服务。</span><span class="sxs-lookup"><span data-stu-id="4cd75-120">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="4cd75-121">为企业添加各个员工：</span><span class="sxs-lookup"><span data-stu-id="4cd75-121">Add individual staff members for the business:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. <span data-ttu-id="4cd75-122">定义企业提供的每项服务：</span><span class="sxs-lookup"><span data-stu-id="4cd75-122">Define each service offered by the business:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="4cd75-123">发布企业的日程安排页面，让客户和企业经营者开始预约：</span><span class="sxs-lookup"><span data-stu-id="4cd75-123">Publish the scheduling page for the business, to let customers and business operators start booking appointments:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="4cd75-124">通常，若要列出 Microsoft 365 租户中的所有预订企业：</span><span class="sxs-lookup"><span data-stu-id="4cd75-124">In general, to list all the booking businesses in the Microsoft 365 tenant:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="4cd75-125">常见用例</span><span class="sxs-lookup"><span data-stu-id="4cd75-125">Common use cases</span></span> 

<span data-ttu-id="4cd75-126">下表列出了 Bookings API 中的常见企业操作。</span><span class="sxs-lookup"><span data-stu-id="4cd75-126">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="4cd75-127">用例</span><span class="sxs-lookup"><span data-stu-id="4cd75-127">Use cases</span></span>        | <span data-ttu-id="4cd75-128">REST 资源</span><span class="sxs-lookup"><span data-stu-id="4cd75-128">REST resources</span></span> | <span data-ttu-id="4cd75-129">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4cd75-129">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="4cd75-130">创建、获取、更新或删除企业</span><span class="sxs-lookup"><span data-stu-id="4cd75-130">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="4cd75-131">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="4cd75-131">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="4cd75-132">bookingBusiness 的方法</span><span class="sxs-lookup"><span data-stu-id="4cd75-132">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="4cd75-133">更新日程安排策略</span><span class="sxs-lookup"><span data-stu-id="4cd75-133">Update the scheduling policy</span></span> | [<span data-ttu-id="4cd75-134">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4cd75-134">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="4cd75-135">更新 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="4cd75-135">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="4cd75-136">添加、获取、更新或删除员工</span><span class="sxs-lookup"><span data-stu-id="4cd75-136">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="4cd75-137">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="4cd75-137">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="4cd75-138">bookingStaffMember 的方法</span><span class="sxs-lookup"><span data-stu-id="4cd75-138">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="4cd75-139">添加、获取、更新或删除服务</span><span class="sxs-lookup"><span data-stu-id="4cd75-139">Add, get, update, or delete services</span></span> | [<span data-ttu-id="4cd75-140">bookingService</span><span class="sxs-lookup"><span data-stu-id="4cd75-140">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="4cd75-141">bookingService 的方法</span><span class="sxs-lookup"><span data-stu-id="4cd75-141">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="4cd75-142">发布或取消发布日程安排页面</span><span class="sxs-lookup"><span data-stu-id="4cd75-142">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="4cd75-143">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="4cd75-143">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="4cd75-144">发布</span><span class="sxs-lookup"><span data-stu-id="4cd75-144">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="4cd75-145">取消发布</span><span class="sxs-lookup"><span data-stu-id="4cd75-145">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="4cd75-146">创建、获取、更新、删除或取消约会</span><span class="sxs-lookup"><span data-stu-id="4cd75-146">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="4cd75-147">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="4cd75-147">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="4cd75-148">bookingAppointment 的方法</span><span class="sxs-lookup"><span data-stu-id="4cd75-148">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="4cd75-149">获取某个日期范围内的约会</span><span class="sxs-lookup"><span data-stu-id="4cd75-149">Get appointments in a date range</span></span> | [<span data-ttu-id="4cd75-150">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="4cd75-150">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="4cd75-151">列出 Bookings 日历视图</span><span class="sxs-lookup"><span data-stu-id="4cd75-151">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="4cd75-152">获取货币</span><span class="sxs-lookup"><span data-stu-id="4cd75-152">Get currency</span></span> | [<span data-ttu-id="4cd75-153">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="4cd75-153">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="4cd75-154">bookingCurrency 的方法</span><span class="sxs-lookup"><span data-stu-id="4cd75-154">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |

## <a name="whats-new"></a><span data-ttu-id="4cd75-155">最近更新</span><span class="sxs-lookup"><span data-stu-id="4cd75-155">What's new</span></span>
<span data-ttu-id="4cd75-156">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="4cd75-156">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="see-also"></a><span data-ttu-id="4cd75-157">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4cd75-157">See also</span></span>

- <span data-ttu-id="4cd75-158">尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="4cd75-158">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="4cd75-159">请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/partners)。</span><span class="sxs-lookup"><span data-stu-id="4cd75-159">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/partners).</span></span>
- <span data-ttu-id="4cd75-160">了解如何在 Microsoft Graph 中选择[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cd75-160">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>


