---
title: Microsoft Bookings API 概述（预览版）
description: Microsoft Bookings 提供了联机移动应用，可便于组织及他们的客户和用户轻松高效地安排约会。
author: arvindmicrosoft
ms.localizationpriority: high
ms.prod: bookings
ms.custom: scenarios:getting-started
ms.openlocfilehash: 3caf87b95533088bb1d0968fbcad6050c54fa51d
ms.sourcegitcommit: 11be55b40804b07f4c422f09f601afa97c7d31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2021
ms.locfileid: "60256506"
---
# <a name="microsoft-bookings-api-overview-preview"></a>Microsoft Bookings API 概述（预览版）

Microsoft Bookings 提供了联机移动应用，可便于小型企业及其客户轻松高效地安排约会。 任何提供预约服务的组织（如大型企业、汽车维修店、发廊和律师事务所）都可以从管理他们的预订中受益，从而有时间来做一些有助于业务增长的更重要的任务。 Microsoft Bookings 适用于拥有 Microsoft 365 商业高级版订阅的企业组织和企业。

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>为什么使用 Microsoft Graph 与 Microsoft Bookings 集成？

### <a name="streamline-appointment-booking"></a>简化预约流程
即使不在电话旁边或在下班时间，业务经营者也绝不会错过客户预订。 客户可以[查看可用服务](/graph/api/bookingbusiness-list-services)，并且随时都能在日程安排页、业务网站或 Facebook 上直接[预订约会](/graph/api/bookingbusiness-post-appointments)。 

业务经营者可以随时随地接受预订，方式包括上网、移动应用、面对面或通过电话。 他们可以[重新安排](/graph/api/bookingappointment-update)、[取消](/graph/api/bookingappointment-cancel)现有预订或将其[重新分配](/graph/api/bookingappointment-update)给其他可用的员工成员。 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>减少失约的情况并提高员工的工作效率
企业经营者可以指定[日程安排策略](/graph/api/resources/bookingschedulingpolicy)，其中包含最低限度的预订和取消通知，客户可自行计划或重新计划预约。 自动的预约确认和提醒会减少失约情况，并让员工更好地利用他们的生产时间。 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>从任何位置管理客户信息和关系
完成预约时将自动验证客户是否已在[客户列表](/graph/api/bookingbusiness-list-customers)上，并根据情况将客户的姓名和电子邮件地址[添加](/graph/api/bookingbusiness-post-customers)到该列表。 这可使企业经营者方便地与客户保持联系，并定期发送新闻稿或其他宣传材料。

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>在 Microsoft Graph 中集成工作效率和团队协作服务
使用相同的统一 Microsoft Graph REST 端点，可以访问 Bookings API，并[与 Microsoft 365 的最佳功能进行集成](overview-major-services.md)以支持更丰富的应用场景。 例如，可以使用 [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) 跟踪和分析企业财务数据并生成专业的报表，或者使用 [SharePoint](sharepoint-concept-overview.md) 或 [Microsoft Teams](teams-concept-overview.md) 来增强团队协作。

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

请参阅 [Microsoft Graph beta 中的 Microsoft Bookings API](/graph/api/resources/booking-api-overviewa)。


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [Microsoft Bookings](https://support.office.com/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) 和其他 [Microsoft 365 商业版应用](https://www.microsoft.com/microsoft-365)。
- 在 Microsoft Graph 中[使用 Bookings API](/graph/api/resources/booking-api-overview)。

