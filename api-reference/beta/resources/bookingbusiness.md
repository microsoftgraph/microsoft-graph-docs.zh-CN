---
title: bookingBusiness 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: fb8b79b4c728236ebc8231bae5da74e65466c20c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861633"
---
# <a name="bookingbusiness-resource-type"></a>bookingBusiness 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
代表在 Microsoft 预订业务。 这是 Microsoft 的预定 API 中的顶级对象。 它包含业务信息和约会、 客户、 服务和人员等的相关的业务对象。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 bookingBusinesses](../api/bookingbusiness-list.md) | [bookingBusiness](bookingbusiness.md)集合 |为租户中获取 bookingbusiness 对象的集合。 |
|[创建 bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | 创建新的 Microsoft 预订业务。 |
|[获取 bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |读取属性和 bookingBusiness 对象的关系。|
|[Update](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |更新**bookingBusiness**对象中的属性。 |
|[删除](../api/bookingbusiness-delete.md) | 无 |删除**bookingBusiness**对象。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| 通过发布到约会集合中创建新 bookingAppointment。|
|[列表约会](../api/bookingbusiness-list-appointments.md) |[bookingAppointment](bookingappointment.md)集合| 获取 bookingAppointment 对象集合。|
|[创建 bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| 通过发布到客户集合中创建新 bookingCustomer。|
|[列出的客户](../api/bookingbusiness-list-customers.md) |[bookingCustomer](bookingcustomer.md)集合| 获取 bookingCustomer 对象集合。|
|[创建 bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| 通过发布到的服务集创建新 bookingService。|
|[列表服务](../api/bookingbusiness-list-services.md) |[bookingService](bookingservice.md)集合| 获取 bookingService 对象集合。|
|[创建 bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| 通过发布到 staffMembers 集合中创建新 bookingStaffMember。|
|[列表 staffMembers](../api/bookingbusiness-list-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)集合| 获取 bookingStaffMember 对象集合。|
|[列出 calendarView](../api/bookingbusiness-list-calendarview.md)|[bookingAppointment](bookingappointment.md)集合|获取指定的日期范围内发生**bookingAppointment**对象的集合。|
|[发布](../api/bookingbusiness-publish.md)|无|将此业务的计划页提供给外部的客户。 **IsPublished**属性设置为 true，并**publicUrl**属性设为计划页的 URL。|
|[取消发布](../api/bookingbusiness-unpublish.md)|无| 对外部客户进行此业务计划页上不可用。 **IsPublished**属性设置为 false，并**publicUrl**属性设为 null。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|业务街道地址。 **Address**属性，以及**电话**和**webSiteUrl**，显示页脚中的企业计划页。|
|工作时间|[bookingWorkHours](bookingworkhours.md)集合|业务操作的时间点。|
|businessType|字符串|业务类型。|
|defaultCurrencyIso|字符串|企业中运行 Microsoft 预订的货币代码。|
|displayName|字符串|业务，接口与客户的名称。 此名称将显示在业务计划页的顶部。|
|email|字符串|业务电子邮件地址。|
|id|字符串|业务唯一的编程标识符。 此为只读属性。|
|isPublished|布尔|计划页上进行了可对外部客户。 使用**发布**和**取消发布**操作来设置此属性。 此为只读属性。|
|phone|String|业务电话号码。 **电话**属性，以及**地址**和**webSiteUrl**，显示页脚中的企业计划页。|
|publicUrl|字符串|计划页，其中您[发布](../api/bookingbusiness-publish.md)或[取消公开](../api/bookingbusiness-unpublish.md)后页上设置的 URL。 此为只读属性。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|指定如何创建此业务预订。|
|webSiteUrl|字符串|业务网站的 URL。 **WebSiteUrl**属性，以及**地址**，**电话**，显示在业务计划页的页脚。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|appointments|[bookingAppointment](bookingappointment.md)集合| 此业务的所有约会。 只读。 可为 Null。|
|calendarView|[bookingAppointment](bookingappointment.md)集合| 一组约会的指定的日期范围中的此业务。 只读。 可为 Null。|
|客户|[bookingCustomer](bookingcustomer.md)集合| 此业务的所有客户。 只读。 可为 Null。|
|服务|[bookingService](bookingservice.md)集合| 此业务提供的所有服务。 只读。 可为 Null。|
|staffMembers|[bookingStaffMember](bookingstaffmember.md)集合| 所有员工成员在此业务提供服务。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
