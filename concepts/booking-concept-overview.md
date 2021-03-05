---
title: Microsoft Bookings API 概述（预览版）
description: Microsoft Bookings 提供了联机移动应用，可便于组织及他们的客户和用户轻松高效地安排约会。
author: arvindmicrosoft
localization_priority: Priority
ms.prod: bookings
ms.custom: scenarios:getting-started
ms.openlocfilehash: 5dfd34bb7defd6f525a5869221ce2c0215826da6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432863"
---
# <a name="microsoft-bookings-api-overview-preview"></a><span data-ttu-id="68887-103">Microsoft Bookings API 概述（预览版）</span><span class="sxs-lookup"><span data-stu-id="68887-103">Microsoft Bookings API overview (preview)</span></span>

<span data-ttu-id="68887-104">Microsoft Bookings 提供了联机移动应用，可便于小型企业及其客户轻松高效地安排约会。</span><span class="sxs-lookup"><span data-stu-id="68887-104">Microsoft Bookings provides online and mobile apps that make appointment scheduling simple and efficient for small businesses and their customers.</span></span> <span data-ttu-id="68887-105">任何提供预约服务的组织（如大型企业、汽车维修店、发廊和律师事务所）都可以从管理他们的预订中受益，从而有时间来做一些有助于业务增长的更重要的任务。</span><span class="sxs-lookup"><span data-stu-id="68887-105">Any organization that provides service on an appointment basis, such as large scale enterprise companies, auto repair shops, hair salons, and law firms, can benefit from having their bookings managed so as to free up time for the more important task to grow their business.</span></span> <span data-ttu-id="68887-106">Microsoft Bookings 适用于拥有 Microsoft 365 商业高级版订阅的企业组织和企业。</span><span class="sxs-lookup"><span data-stu-id="68887-106">Microsoft Bookings is available to enterprise organizations and businesses that have a Microsoft 365 Business Premium subscription.</span></span>

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a><span data-ttu-id="68887-107">为什么使用 Microsoft Graph 与 Microsoft Bookings 集成？</span><span class="sxs-lookup"><span data-stu-id="68887-107">Why integrate with Microsoft Bookings using Microsoft Graph?</span></span>

### <a name="streamline-appointment-booking"></a><span data-ttu-id="68887-108">简化预约流程</span><span class="sxs-lookup"><span data-stu-id="68887-108">Streamline appointment booking</span></span>
<span data-ttu-id="68887-109">即使不在电话旁边或在下班时间，业务经营者也绝不会错过客户预订。</span><span class="sxs-lookup"><span data-stu-id="68887-109">A business operator may never miss a customer booking when away from the phone or the business is closed.</span></span> <span data-ttu-id="68887-110">客户可以[查看可用服务](/graph/api/bookingbusiness-list-services?view=graph-rest-beta)，并且随时都能在日程安排页、业务网站或 Facebook 上直接[预订约会](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="68887-110">Customers can [see the available services](/graph/api/bookingbusiness-list-services?view=graph-rest-beta) and [book appointments](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta) any time directly on the scheduling page, on the business web site or Facebook.</span></span> 

<span data-ttu-id="68887-111">业务经营者可以随时随地接受预订，方式包括上网、移动应用、面对面或通过电话。</span><span class="sxs-lookup"><span data-stu-id="68887-111">Business operators can take bookings anywhere, on the web or a mobile app, in-person or on the phone.</span></span> <span data-ttu-id="68887-112">他们可以[重新安排](/graph/api/bookingappointment-update?view=graph-rest-beta)、[取消](/graph/api/bookingappointment-cancel?view=graph-rest-beta)现有预订或将其[重新分配](/graph/api/bookingappointment-update?view=graph-rest-beta)给其他可用的员工成员。</span><span class="sxs-lookup"><span data-stu-id="68887-112">They can [reschedule](/graph/api/bookingappointment-update?view=graph-rest-beta), [cancel](/graph/api/bookingappointment-cancel?view=graph-rest-beta), or [re-assign](/graph/api/bookingappointment-update?view=graph-rest-beta) an existing booking to another available staff member.</span></span> 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a><span data-ttu-id="68887-113">减少失约的情况并提高员工的工作效率</span><span class="sxs-lookup"><span data-stu-id="68887-113">Reduce no-shows and increase productivity of the staff</span></span>
<span data-ttu-id="68887-114">企业经营者可以指定[日程安排策略](/graph/api/resources/bookingschedulingpolicy?view=graph-rest-beta)，其中包含最低限度的预订和取消通知，客户可自行计划或重新计划预约。</span><span class="sxs-lookup"><span data-stu-id="68887-114">Business operators can specify [scheduling policies](/graph/api/resources/bookingschedulingpolicy?view=graph-rest-beta) that include minimum notice for bookings and cancellations, and customers can schedule or reschedule appointments themselves.</span></span> <span data-ttu-id="68887-115">自动的预约确认和提醒会减少失约情况，并让员工更好地利用他们的生产时间。</span><span class="sxs-lookup"><span data-stu-id="68887-115">Automated appointment confirmations and reminders decrease no-shows, and let the staff make better use of their production hours.</span></span> 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a><span data-ttu-id="68887-116">从任何位置管理客户信息和关系</span><span class="sxs-lookup"><span data-stu-id="68887-116">Manage customer information and relationships from anywhere</span></span>
<span data-ttu-id="68887-117">完成预约时将自动验证客户是否已在[客户列表](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta)上，并根据情况将客户的姓名和电子邮件地址[添加](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta)到该列表。</span><span class="sxs-lookup"><span data-stu-id="68887-117">Completing an appointment automatically verifies if the customer is already on the [customer list](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta), and [adds](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta) the customer's name and email address to the list if necessary.</span></span> <span data-ttu-id="68887-118">这可使企业经营者方便地与客户保持联系，并定期发送新闻稿或其他宣传材料。</span><span class="sxs-lookup"><span data-stu-id="68887-118">This makes it convenient for business operators to stay in touch with their customers, and send periodic newsletters or other promotional material.</span></span>

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a><span data-ttu-id="68887-119">在 Microsoft Graph 中集成工作效率和团队协作服务</span><span class="sxs-lookup"><span data-stu-id="68887-119">Integrate with productivity and team collaboration services in Microsoft Graph</span></span>
<span data-ttu-id="68887-120">使用相同的统一 Microsoft Graph REST 端点，可以访问 Bookings API，并[与 Microsoft 365 的最佳功能进行集成](overview-major-services.md)以支持更丰富的应用场景。</span><span class="sxs-lookup"><span data-stu-id="68887-120">Using the same unified Microsoft Graph REST endpoint, you can access the Bookings API and [integrate with the best of Microsoft 365](overview-major-services.md) to support richer scenarios.</span></span> <span data-ttu-id="68887-121">例如，可以使用 [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) 跟踪和分析企业财务数据并生成专业的报表，或者使用 [SharePoint](sharepoint-concept-overview.md) 或 [Microsoft Teams](teams-concept-overview.md) 来增强团队协作。</span><span class="sxs-lookup"><span data-stu-id="68887-121">For example, you can use [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) to track and analyze business financial data, and generate professional reports, or use [SharePoint](sharepoint-concept-overview.md) or [Microsoft Teams](teams-concept-overview.md) to enhance team collaboration.</span></span>

## <a name="api-reference"></a><span data-ttu-id="68887-122">API 参考</span><span class="sxs-lookup"><span data-stu-id="68887-122">API reference</span></span>
<span data-ttu-id="68887-123">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="68887-123">Looking for the API reference for this service?</span></span>

<span data-ttu-id="68887-124">请参阅 [Microsoft Graph beta 中的 Microsoft Bookings API](/graph/api/resources/booking-api-overview?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="68887-124">See [Microsoft Bookings API in Microsoft Graph beta](/graph/api/resources/booking-api-overview?view=graph-rest-beta).</span></span>


## <a name="next-steps"></a><span data-ttu-id="68887-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="68887-125">Next steps</span></span>

<span data-ttu-id="68887-126">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="68887-126">Learn more about:</span></span>

- <span data-ttu-id="68887-127">[Microsoft Bookings](https://support.office.com/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) 和其他 [Microsoft 365 商业版应用](https://support.office.com/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US)。</span><span class="sxs-lookup"><span data-stu-id="68887-127">[Microsoft Bookings](https://support.office.com/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) and other [Microsoft 365 business apps](https://support.office.com/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US).</span></span>
- <span data-ttu-id="68887-128">在 Microsoft Graph 中[使用 Bookings API](/graph/api/resources/booking-api-overview?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="68887-128">[Using the Bookings API](/graph/api/resources/booking-api-overview?view=graph-rest-beta) in Microsoft Graph.</span></span>

