---
title: bookingBusiness 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 03790cfe39ef2de463ae843ba6b18cd6d91e754d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543846"
---
# <a name="bookingbusiness-resource-type"></a>bookingBusiness 资源类型

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示 Microsoft 预订中的企业。 这是 Microsoft 记帐 API 中的顶级对象。 它包含业务信息和相关业务对象, 如约会、客户、服务和员工成员。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 errorexceededfindcountlimit](../api/bookingbusiness-list.md) | [bookingBusiness](bookingbusiness.md)集合 |获取租户中的 bookingbusiness 对象的集合。 |
|[创建 bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | 创建新的 Microsoft 预订业务。 |
|[获取 bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |读取 bookingBusiness 对象的属性和关系。|
|[更新](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |更新**bookingBusiness**对象中的属性。 |
|[删除](../api/bookingbusiness-delete.md) | 无 |删除**bookingBusiness**对象。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| 通过发布到 "约会" 集合创建新的 bookingAppointment。|
|[列出约会](../api/bookingbusiness-list-appointments.md) |[bookingAppointment](bookingappointment.md)集合| 获取 bookingAppointment 对象集合。|
|[创建 bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| 通过发布到 "客户" 集合创建新的 bookingCustomer。|
|[列出客户](../api/bookingbusiness-list-customers.md) |[bookingCustomer](bookingcustomer.md)集合| 获取 bookingCustomer 对象集合。|
|[创建 bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| 通过发布到服务集合创建新的 bookingService。|
|[列出服务](../api/bookingbusiness-list-services.md) |[bookingService](bookingservice.md)集合| 获取 bookingService 对象集合。|
|[创建 bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| 通过发布到 staffMembers 集合创建新的 bookingStaffMember。|
|[列出 staffMembers](../api/bookingbusiness-list-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)集合| 获取 bookingStaffMember 对象集合。|
|[List calendarView](../api/bookingbusiness-list-calendarview.md)|[bookingAppointment](bookingappointment.md)集合|获取在指定日期范围内发生的**bookingAppointment**对象的集合。|
|[发布](../api/bookingbusiness-publish.md)|无|使此业务的日程安排页面对外部客户可用。 将**isPublished**属性设置为 true, 并将**publicUrl**属性设置为计划页面的 URL。|
|[取消发布](../api/bookingbusiness-unpublish.md)|无| 使此业务的计划页面对外部客户不可用。 将**isPublished**属性设置为 false, 并将**publicUrl**属性设置为 null。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|企业的街道地址。 **address**属性以及**手机**和**webSiteUrl**将显示在 "业务计划" 页的页脚中。|
|businessHours|[bookingWorkHours](bookingworkhours.md)集合|业务的运行时间。|
|businessType|String|企业的类型。|
|defaultCurrencyIso|String|业务在 Microsoft 预订中所运行的货币的代码。|
|displayName|String|业务的名称, 与客户的接口。 此名称显示在 "业务计划" 页的顶部。|
|email|字符串|企业的电子邮件地址。|
|id|String|企业的唯一编程标识符。 只读。|
|isPublished|布尔值|计划页面已提供给外部客户。 使用 "**发布**" 和 "**取消发布**" 操作设置此属性。 只读。|
|phone|String|企业的电话号码。 **phone**属性, 以及**address**和**webSiteUrl**将显示在 "业务计划" 页的页脚中。|
|publicUrl|String|计划页面的 URL, 在[发布](../api/bookingbusiness-publish.md)或[取消](../api/bookingbusiness-unpublish.md)发布页面之后设置。 只读。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|指定如何为此公司创建预订。|
|webSiteUrl|String|业务网站的 URL。 **webSiteUrl**属性 (与**address**、 **phone**) 显示在 "业务计划" 页的页脚中。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|appointments|[bookingAppointment](bookingappointment.md)集合| 此业务的所有约会。 只读。 可为 Null。|
|calendarView|[bookingAppointment](bookingappointment.md)集合| 在指定日期范围内此公司的一组约会。 只读。 可为 Null。|
|各地|[bookingCustomer](bookingcustomer.md)集合| 此业务的所有客户。 只读。 可为 Null。|
|服务行业|[bookingService](bookingservice.md)集合| 此业务提供的所有服务。 只读。 可为 Null。|
|staffMembers|[bookingStaffMember](bookingstaffmember.md)集合| 在此公司中提供服务的所有教职员工成员。 只读。 可为 Null。|

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingbusiness.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
