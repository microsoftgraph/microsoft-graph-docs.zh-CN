---
title: bookingBusiness 资源类型
description: 表示Microsoft Bookings中的一家企业。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: ccafc23fc8a1276ec7ffa9df4b0b2c8769142e32
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856293"
---
# <a name="bookingbusiness-resource-type"></a>bookingBusiness 资源类型

命名空间：microsoft.graph

表示Microsoft Bookings中的一家企业。 这是Microsoft Bookings API 中的顶级对象。 它包含业务信息和相关的业务对象，例如约会、客户、服务和员工。

## <a name="methods"></a>方法

| 方法  | 返回类型 |Description|
|:---------------|:--------|:----------|
|[列出 bookingBusinesses](../api/bookingbusiness-list.md) | [bookingBusiness](bookingbusiness.md) 集合 |获取租户中的 **bookingBusiness** 对象集合。 |
|[创建 bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | 创建新的Microsoft Bookings业务。 |
|[获取 bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |读取 **bookingBusiness** 对象的属性和关系。|
|[更新](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |更新 **bookingBusiness** 对象中的属性。 |
|[删除](../api/bookingbusiness-delete.md) | 无 |删除 **bookingBusiness** 对象。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| 通过发布到约会集合来创建新的 **bookingAppointment** 。|
|[列出约会](../api/bookingbusiness-list-appointments.md) |[bookingAppointment](bookingappointment.md) 集合| 获取 **bookingAppointment** 对象集合。|
|[创建 bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| 通过发布到客户集合来创建新的 **bookingCustomer** 。|
|[列出客户](../api/bookingbusiness-list-customers.md) |[bookingCustomer](bookingcustomer.md) 集合| 获取 **bookingCustomer** 对象集合。|
|[创建 bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| 通过发布到服务集合来创建新的 **bookingService** 。|
|[列出服务](../api/bookingbusiness-list-services.md) |[bookingService](bookingservice.md) 集合| 获取 **bookingService** 对象集合。|
|[创建 bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| 通过发布到 staffMembers 集合来创建新的 **bookingStaffMember** 。|
|[列出 staffMembers](../api/bookingbusiness-list-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md) 集合| 获取 **bookingStaffMember** 对象集合。|
|[列出 customQuestions](../api/bookingbusiness-list-customquestions.md)|[bookingCustomQuestion](../resources/bookingcustomquestion.md) 集合|从 **customQuestions** 导航属性获取 **bookingCustomQuestion** 资源。|
|[创建 bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md)|[bookingCustomQuestion](../resources/bookingcustomquestion.md)|创建新的 **bookingCustomQuestion** 对象。|
|[List calendarView](../api/bookingbusiness-list-calendarview.md)|[bookingAppointment](bookingappointment.md) 集合|获取在指定日期范围内发生的 **bookingAppointment** 对象的集合。|
|[发布](../api/bookingbusiness-publish.md)|无|使此业务的计划页可供外部客户使用。 将 **isPublished** 属性设置为 `true`**publicUrl** 属性，并将其设置为计划页的 URL。|
|[取消发布](../api/bookingbusiness-unpublish.md)|无| 使此业务的计划页不适用于外部客户。 将 **isPublished** 属性设置为 `false`**publicUrl** 属性`null`。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|企业的街道地址。 **地址** 属性以及 **电话** 和 **webSiteUrl** 显示在业务计划页面的页脚中。 v1.0 不支持 physicalAddress 的属性 **类型** 。 在内部，我们将地址映射到类型 `others`。|
|businessHours|[bookingWorkHours](bookingworkhours.md) 集合|业务运营时间。|
|businessType|String|业务类型。|
|defaultCurrencyIso|String|业务在Microsoft Bookings上运营的货币的代码。|
|displayName|String|与客户接口的业务名称。 此名称显示在业务计划页面的顶部。|
|email|String|业务的电子邮件地址。|
|id|String|业务的唯一编程标识符。 只读。|
|isPublished|Boolean|计划页已提供给外部客户。 使用 **发布** 和 **取消发布** 操作设置此属性。 只读。|
|phone|String|企业的电话号码。 **手机** 属性以及 **地址** 和 **webSiteUrl** 显示在业务计划页面的页脚中。|
|publicUrl|String|计划页的 URL，该 URL 是在 [发布](../api/bookingbusiness-publish.md) 或 [取消发布](../api/bookingbusiness-unpublish.md) 页面后设置的。 只读。|
|schedulePolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|指定如何为此业务创建预订。|
|webSiteUrl|String|业务网站的 URL。 **WebSiteUrl** 属性以及 **地址**、**电话** 显示在业务计划页面的页脚中。|

## <a name="relationships"></a>关系

| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|appointments|[bookingAppointment](bookingappointment.md) 集合| 此业务的所有约会。 只读。 可为 NULL。|
|calendarView|[bookingAppointment](bookingappointment.md) 集合| 此业务在指定日期范围内的约会集。 只读。 可为 NULL。|
|客户|[bookingCustomer](bookingcustomer.md) 集合| 此业务的所有客户。 只读。 可为 NULL。|
|customQuestions|[bookingCustomQuestion](../resources/bookingcustomquestion.md) 集合| 此业务的所有自定义问题。 只读。 可为 NULL。|
|服务|[bookingService](bookingservice.md) 集合| 此业务提供的所有服务。 只读。 可为 NULL。|
|staffMembers|[bookingStaffMember](bookingstaffmember.md) 集合| 在此业务中提供服务的所有员工。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingBusiness"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "businessType": "String",
  "defaultCurrencyIso": "String",
  "displayName": "String",
  "email": "String",
  "id": "String (identifier)",
  "isPublished": true,
  "phone": "String",
  "publicUrl": "String",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "webSiteUrl": "String"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


