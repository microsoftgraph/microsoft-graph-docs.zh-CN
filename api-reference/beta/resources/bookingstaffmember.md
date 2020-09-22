---
title: bookingStaffMember 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 82af39c9b64d7970d92a364199404149928b7b09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071722"
---
# <a name="bookingstaffmember-resource-type"></a>bookingStaffMember 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示在 [bookingBusiness](bookingbusiness.md)中提供服务的教职员工成员。

教职员工成员可以是配置了预订业务的 Microsoft 365 租户的一部分，也可以使用来自其他电子邮件提供商的电子邮件服务。

预订约会时，预订 API 会考虑以下设置以确定教职员工成员的可用性： 

1. 默认情况下，业务运营的时间 ([bookingBusiness](bookingbusiness.md)实体) 的**businessHours**属性表示教职员工成员的正式可用性。
2. 如果 **useBusinessHours** 为 false，则教职员工成员的特定工作时间 (**WorkingHours** 属性的 **bookingStaffmember** 实体) 表示该成员的常规可用性。
3. 如果 **availabilityIsAffectedByPersonalCalendar** 为 true，则预订 API 将首先查看教职员工成员的可用小时数 (由 #1 或 #2) 决定，并在进行预定前在教职员工成员的个人日历中验证这些小时内的可用性。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出教职员工成员](../api/bookingbusiness-list-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) 集合 | 获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**对象的列表。 |
|[创建 bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md) 集合 | 在指定的[bookingbusiness](../resources/bookingbusiness.md)中创建新的**bookingStaffMember** 。 |
|[获取 bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**的属性和关系。|
|[更新](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |更新指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**的属性。|
|[删除](../api/bookingstaffmember-delete.md) | 无 |删除指定 [bookingbusiness](../resources/bookingbusiness.md)中的教职员工成员。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|如果为 True，则表示如果教职员工成员是 Microsoft 365 用户，则预订 API 将在进行预订前验证员工在 Microsoft 365 的个人日历中的可用性。 |
|colorIndex|Int32|标识代表教职员工成员的颜色。 该颜色对应于预订应用中的 " **员工详细信息** " 页上的调色板。|
|displayName|String|向客户显示的教职员工成员的姓名。 必需。|
|emailAddress|String|教职员工成员的电子邮件地址。 这可以与公司在同一 Microsoft 365 租户中，也可以位于不同的电子邮件域中。 如果在企业的计划策略中将 **sendConfirmationsToOwner** 属性设置为 true，则可以使用此电子邮件地址。 必需。|
|id|String| 以 GUID 格式的教职员工成员的 ID。 只读。|
|role|string| 企业中教职员工成员的角色。 可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。 必需。|
|useBusinessHours|Boolean|如果为 True，则表示教职员工成员的可用性是在企业的 **businessHours** 属性中指定的。 False 表示可用性由教职员工成员的 **workingHours** 属性设置决定。|
|workingHours|[bookingWorkHours](bookingworkhours.md) 集合|教职员工成员可用于预订的一周中每一天的小时数。 默认情况下，它们被初始化为与企业的 **businessHours** 属性相同。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


