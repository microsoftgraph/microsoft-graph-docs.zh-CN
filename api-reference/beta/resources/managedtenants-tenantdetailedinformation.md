---
title: tenantDetailedInformation 资源类型
description: 表示托管租户的详细信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 40aa157b12ccef64b6eb7ab6c92349a3e74745f8
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402273"
---
# <a name="tenantdetailedinformation-resource-type"></a>tenantDetailedInformation 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 tenantDetailedInformation](../api/managedtenants-managedtenant-list-tenantsdetailedinformation.md)|[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 集合|获取 [tenantDetailedInformation 对象](../resources/managedtenants-tenantdetailedinformation.md) 及其属性的列表。|
|[获取 tenantDetailedInformation](../api/managedtenants-tenantdetailedinformation-get.md)|[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|读取 [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|城市|String|托管租户所在的城市。 可选。 只读。|
|countryCode|String|托管租户所在的国家/地区的代码。 可选。 只读。|
|countryName|String|托管租户所在的国家/地区的名称。 可选。 只读。|
|defaultDomainName|String|托管租户的默认域名。 可选。 只读。|
|displayName|String|托管显示名称租户的租户。|
|id|String|此实体的唯一标识符。 必填。 只读。|
|industryName|String|与托管租户关联的业务行业。 可选。 只读。|
|region|String|托管租户所在的区域。 可选。 只读。|
|segmentName|String|与托管租户关联的业务部门。 可选。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。|
|verticalName|String|与托管租户关联的垂直。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "defaultDomainName": "String",
  "countryName": "String",
  "countryCode": "String",
  "city": "String",
  "region": "String",
  "verticalName": "String",
  "industryName": "String",
  "segmentName": "String"
}
```

