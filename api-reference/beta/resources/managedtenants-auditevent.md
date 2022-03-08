---
title: auditEvent 资源类型
description: 表示托管租户的审核Microsoft 365 Lighthouse。
author: vkumar2015
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d0a6097178f160fd305060a4a7d6a289b184228c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338340"
---
# <a name="auditevent-resource-type"></a>auditEvent 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的审核Microsoft 365 Lighthouse。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 auditEvents](../api/managedtenants-managedtenant-list-auditevents.md)|[microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md) 集合|获取 [auditEvent](../resources/managedtenants-auditevent.md) 对象及其属性的列表。|
|[获取 auditEvent](../api/managedtenants-auditevent-get.md)|[microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md)|读取 [auditEvent 对象的属性和](../resources/managedtenants-auditevent.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|activity|String|一个字符串，它唯一地表示发生的操作。 必需项。 只读。|
|activityDateTime|DateTimeOffset|活动发生的时间。 必需项。 只读。|
|activityId|字符串|进行审核事件的活动请求的标识符。 必需项。 只读。|
|“类别”|String|表示活动的逻辑分组的类别。 必需项。 只读。|
|httpVerb|字符串|进行 API 请求时所使用的 HTTP 谓词。 必需项。 只读。|
|id|String|审核事件的唯一标识符。 必需项。 只读。|
|initiatedByAppId|字符串|用于提出请求的应用的标识符。 必需项。 只读。|
|initiatedByUpn|String|发起活动的用户的 UPN。 必需项。 只读。|
|initiatedByUserId|String|发起活动的用户的标识符。 必需项。 只读。|
|ipAddress|String|活动发起位置的 IP 地址。 这可能是 IPv4 或 IPv6 地址。 必需项。 只读。|
|requestBody|String|原始 HTTP 请求正文。 可能会删除某些敏感信息。|
|requestUrl|String|原始 HTTP 请求 URL。 必需项。 只读。|
|tenantIds|字符串|受此Azure Active Directory影响的托管租户的租户标识符集合。[](../resources/managedtenants-tenant.md) 此参数的格式设置为逗号分隔值的列表。 必需项。 只读。|
|tenantNames|字符串|受此更改影响的租户名称集合。 此参数的格式设置为逗号分隔值的列表。 必需项。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.auditEvent",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.auditEvent",
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityId": "String",
  "category": "String",
  "httpVerb": "String",
  "id": "String (identifier)",
  "initiatedByAppId": "String",
  "initiatedByUpn": "String",
  "initiatedByUserId": "String",
  "ipAddress": "String",
  "requestBody": "String",
  "requestUrl": "String",
  "tenantIds": "String",
  "tenantNames": "String"
}
```

