---
title: bookingBusiness 资源类型
description: 代表 Microsoft Bookings 中的业务。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 76c08ab05575b1f0c52b7af21db787396e8dba63
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524824"
---
# <a name="bookingbusiness-resource-type"></a>bookingBusiness 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
代表 Microsoft Bookings 中的业务。 这是 Microsoft Bookings API 中的顶级对象。 它包含业务信息和相关的业务对象，如约会、客户、服务和员工成员。

继承自 [bookingNamedEntity](bookingnamedentity.md)

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 bookingBusinesses](../api/bookingbusiness-list.md) | [bookingBusiness](bookingbusiness.md) 集合 |获取租户中的 bookingbusiness 对象的集合。 |
|[创建 bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | 创建新的 Microsoft Bookings 业务。 |
|[获取 bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |读取 bookingBusiness 对象的属性和关系。|
|[更新](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |更新 **bookingBusiness 对象中的** 属性。 |
|[删除](../api/bookingbusiness-delete.md) | 无 |删除 **bookingBusiness** 对象。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| 通过发布到约会集合创建新的 bookingAppointment。|
|[列出约会](../api/bookingbusiness-list-appointments.md) |[bookingAppointment](bookingappointment.md) 集合| 获取 bookingAppointment 对象集合。|
|[创建 bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| 通过发布到客户集合创建新的 bookingCustomer。|
|[列出客户](../api/bookingbusiness-list-customers.md) |[bookingCustomer](bookingcustomer.md) 集合| 获取 bookingCustomer 对象集合。|
|[创建 bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| 通过发布到服务集合创建新的 bookingService。|
|[列出服务](../api/bookingbusiness-list-services.md) |[bookingService](bookingservice.md) 集合| 获取 bookingService 对象集合。|
|[创建 bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| 通过发布到 staffMembers 集合创建新的 bookingStaffMember。|
|[列出 staffMembers](../api/bookingbusiness-list-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md) 集合| 获取 bookingStaffMember 对象集合。|
|[列出 customQuestions](../api/bookingbusiness-list-customquestions.md)|[bookingCustomQuestion](../resources/bookingcustomquestion.md) 集合|从 **customQuestions** 导航属性获取 **bookingCustomQuestion** 资源。|
|[创建 bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md)|[bookingCustomQuestion](../resources/bookingcustomquestion.md)|创建新的 **bookingCustomQuestion** 对象。|
|[列出 calendarView](../api/bookingbusiness-list-calendarview.md)|[bookingAppointment](bookingappointment.md) 集合|获取指定日期范围内 **发生的 bookingAppointment** 对象的集合。|
|[发布](../api/bookingbusiness-publish.md)|无|使外部客户可以使用此业务的计划页。 将 **isPublished** 属性设置为 true，将 **publicUrl** 属性设置为计划页的 URL。|
|[取消发布](../api/bookingbusiness-unpublish.md)|无| 使此业务的计划页对外部客户不可用。 将 **isPublished** 属性设置为 false，将 **publicUrl** 属性设置为 null。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|企业街道地址。 **address** 属性与 **phone** 和 **webSiteUrl** 一起显示在业务日程安排页面的页脚中。|
|businessHours|[bookingWorkHours](bookingworkhours.md) 集合|企业运营的小时数。|
|businessType|String|业务类型。|
|defaultCurrencyIso|String|在 Microsoft Bookings 上运营业务的货币代码。|
|displayName|String|与客户交互的业务名称。 此名称显示在业务计划页面的顶部。|
|email|字符串|企业的电子邮件地址。|
|id|String|企业的唯一编程标识符。 只读。|
|isPublished|Boolean|计划页面已提供给外部客户。 使用 **发布****和取消发布** 操作可设置此属性。 只读。|
|phone|String|企业的电话号码。 **phone** 属性与 **address** 和 **webSiteUrl** 一起显示在业务日程安排页面的页脚中。|
|publicUrl|String|计划页面的 URL，在发布或取消[发布页面后](../api/bookingbusiness-unpublish.md)设置。 [](../api/bookingbusiness-publish.md) 只读。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|指定如何为此业务创建预订。|
|webSiteUrl|String|业务网站的 URL。 **webSiteUrl** 属性和 **地址** **、phone** 一起显示在业务日程安排页面的页脚中。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|appointments|[bookingAppointment](bookingappointment.md) 集合| 此业务的所有约会。 只读。 可为 NULL。|
|calendarView|[bookingAppointment](bookingappointment.md) 集合| 该企业在指定的日期范围内约会集。 只读。 可为 NULL。|
|customers|[bookingCustomer](bookingcustomer.md) 集合| 此业务的所有客户。 只读。 可为 NULL。|
|customQuestions|[bookingCustomQuestion](../resources/bookingcustomquestion.md) 集合| 此业务的所有自定义问题。 只读。 可为 NULL。|
|服务|[bookingService](bookingservice.md) 集合| 此企业提供的所有服务。 只读。 可为 NULL。|
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

## <a name="see-also"></a>另请参阅


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


