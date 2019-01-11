---
title: 使用在 Microsoft Graph 中 Microsoft 预订 API
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Priority
ms.openlocfilehash: def9260654baafe1953d629265c4b76a2afd2748
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845533"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>使用在 Microsoft Graph 中 Microsoft 预订 API

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
Microsoft 预订允许小型企业所有者管理客户的预定和通过少量设置的信息。 业务所有者可以提供一组服务的每个业务部门创建一个或多个企业版。 所有者可以设置人员，并指定每个员工成员执行的服务。 客户可以在联机或移动应用程序中的业务书籍特定服务的约会。 预订确保的约会时间保持最新的人员，业务和客户涉及。

以编程方式预订 API 中[bookingBusiness](bookingbusiness.md)涉及以下对象：
 
- 一个或多个[bookingStaffMember](bookingstaffmember.md)对象
- 一个或多个[bookingService](bookingservice.md)对象
- 一套[bookingAppointment](bookingappointment.md)实例
- 一组[bookingCustomer](bookingcustomer.md)对象

## <a name="using-the-bookings-rest-api"></a>使用预订 REST API

预订第一次的业务的客户约会之前逐步完成以下步骤。 请确保您为相应的操作提供适当的[访问令牌](/graph/auth-overview)。

1. 确保业务具有的[Office 365 企业高级版](https://products.office.com/en-us/business/office-365-business-premium)订阅。
2. 创建新**bookingBusiness**通过将 POST 操作发送到的实体集。 至少应指定客户将看到新的业务的名称：<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
POST 响应中返回新**bookingBusiness**的**id**属性用于继续[自定义](../api/bookingbusiness-update.md)业务设置，并添加员工和业务的服务。

3. 添加业务的人员成员：<!-- { "blockType": "ignored" } -->
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
4. 定义由业务提供每个服务：<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. 发布的企业，可以让客户和业务运算符启动预订约会的计划页：<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

通常，列出 Office 365 租户中的所有预订企业： 中<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>常见用例 

下表列出了业务预订 API 中的常见操作。

| 用例        | REST 资源 | 另请参阅 |
|:---------------|:--------|:----------|
| 创建、 获取、 更新或删除业务 | [bookingBusiness](bookingbusiness.md) | [BookingBusiness 方法](bookingbusiness.md#methods) |
| 更新计划策略 | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [更新 bookingBusiness](../api/bookingbusiness-update.md) |
| 添加、 获取、 更新或删除员工成员 | [bookingStaffMember](bookingstaffmember.md) | [BookingStaffMember 方法](bookingstaffmember.md#methods)  |
| 添加、 获取、 更新或删除服务 | [bookingService](bookingservice.md) | [BookingService 方法](bookingservice.md#methods)  |
| 公开或取消公开计划页 | [bookingBusiness](bookingbusiness.md) | [发布](../api/bookingbusiness-publish.md) <br> [取消发布](../api/bookingbusiness-unpublish.md) |
| 创建、 获取、 更新、 删除或取消约会 | [bookingAppointment](bookingappointment.md) | [BookingAppointment 方法](bookingappointment.md#methods)  |
| 获取约会中的日期范围 | [bookingBusiness](bookingbusiness.md) | [列表的预定 calendarView](../api/bookingbusiness-list-calendarview.md) |
| 获取货币 | [bookingCurrency](bookingcurrency.md) | [BookingCurrency 方法](bookingcurrency.md#methods) |


## <a name="see-also"></a>另请参阅

- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。
- 请参阅[一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。
- 了解如何在 Microsoft Graph 中选择[权限](/graph/permissions-reference)。
