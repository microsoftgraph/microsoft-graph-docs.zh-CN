---
title: 使用 Microsoft Graph 中的 Microsoft Bookings API
description: Microsoft Bookings 可让企业组织和小型企业所有者以最少量的设置管理客户预订和信息。
ms.localizationpriority: high
author: arvindmicrosoft
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: 622feed07a5387301be148c926088add62946f25
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58694858"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>使用 Microsoft Graph 中的 Microsoft Bookings API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Bookings 可让企业组织和小型企业所有者以最少量的设置管理客户预订和信息。 企业所有者可以创建一个或多个企业，每个企业都提供一组服务。 所有者可以设置员工，并指定每名员工执行的服务。 客户可以通过在线或移动应用预约该企业中的特定服务。 Bookings 可确保为企业、员工和相关客户保持最新的约会时间。

就编程而言，Bookings API 中的 [bookingBusiness](bookingbusiness.md) 涉及以下对象：

- 一个或多个 [bookingStaffMember](bookingstaffmember.md) 对象
- 一个或多个 [bookingService](bookingservice.md) 对象
- 一组 [bookingAppointment](bookingappointment.md) 实例
- 一组 [bookingCustomer](bookingcustomer.md) 对象

## <a name="using-the-bookings-rest-api"></a>使用 Bookings REST API

第一次客户预约之前，请完成以下步骤。 确保为相应的操作提供适当的[访问令牌](/graph/auth-overview)。

1. 确保企业具有 [Microsoft 365 商业高级版](https://products.office.com/en-us/business/office-365-business-premium)订阅。
2. 通过向实体集发送 POST 操作来创建新的 **bookingBusiness**。 至少应为新企业指定客户将看到的名称：
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
使用 POST 响应中返回的新 **bookingBusiness** 的 **id** 属性继续 [自定义](../api/bookingbusiness-update.md)企业设置，并为企业添加员工和服务。

3. 为企业添加各个员工：
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
4. 定义企业提供的每项服务：
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. 发布企业的日程安排页面，让客户和企业经营者开始预约：
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

通常，若要列出 Microsoft 365 租户中的所有预订企业：
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>常见用例

下表列出了 Bookings API 中的常见企业操作。

| 用例        | REST 资源 | 另请参阅 |
|:---------------|:--------|:----------|
| 创建、获取、更新或删除企业 | [bookingBusiness](bookingbusiness.md) | [bookingBusiness 的方法](bookingbusiness.md#methods) |
| 更新日程安排策略 | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [更新 bookingBusiness](../api/bookingbusiness-update.md) |
| 添加、获取、更新或删除员工 | [bookingStaffMember](bookingstaffmember.md) | [bookingStaffMember 的方法](bookingstaffmember.md#methods)  |
| 添加、获取、更新或删除服务 | [bookingService](bookingservice.md) | [bookingService 的方法](bookingservice.md#methods)  |
| 发布或取消发布日程安排页面 | [bookingBusiness](bookingbusiness.md) | [发布](../api/bookingbusiness-publish.md) <br> [取消发布](../api/bookingbusiness-unpublish.md) |
| 创建、获取、更新、删除或取消约会 | [bookingAppointment](bookingappointment.md) | [bookingAppointment 的方法](bookingappointment.md#methods)  |
| 获取某个日期范围内的约会 | [bookingBusiness](bookingbusiness.md) | [列出 Bookings 日历视图](../api/bookingbusiness-list-calendarview.md) |
| 获取货币 | [bookingCurrency](bookingcurrency.md) | [bookingCurrency 的方法](bookingcurrency.md#methods) |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="see-also"></a>另请参阅

- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。
- 请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/partners)。
- 了解如何在 Microsoft Graph 中选择[权限](/graph/permissions-reference)。


