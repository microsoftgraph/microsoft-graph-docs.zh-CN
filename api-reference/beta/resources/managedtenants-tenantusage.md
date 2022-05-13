---
title: tenantUsage 资源类型
description: 表示上个月托管租户中每个服务的每月活动用户数。 数据的时间段是一个滑动窗口，每天拍摄一次快照。
author: kylewirpel
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f1d568e2218c460aeef9bff54db636f30ac94d07
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398644"
---
# <a name="tenantusage-resource-type"></a>tenantUsage 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示上个月托管租户中每个服务的每月活动用户数。 数据的时间段是一个滑动窗口，每天拍摄一次快照。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 tenantUsage](../api/managedtenants-managedtenant-list-tenantusage.md)|[microsoft.graph.managedTenants.tenantUsage](../resources/managedtenants-tenantusage.md) 集合|获取[托管租户](../resources/managedtenants-managedtenant.md)中[每个服务的每月使用情况数据](../resources/managedtenants-tenantusage.md)。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|租户的唯一标识符。 必填。 只读。|
|reportDateTime|DateTimeOffset|报表在上个月生成的日期。 必填。 只读。|
|serviceUsages|[microsoft.graph.managedTenants.serviceUsage](../resources/managedtenants-serviceusage.md) 集合|租户中每个服务的每月活动用户数。 示例服务： `Excel`， `Exchange`， `Intune`， `Outlook`， `Teams`。 `Word` 必填。 只读。|
|tenantId|String|托管租户的Azure Active Directory[租户](../resources/managedtenants-tenant.md)标识符。 只读。|
|totalActiveUsers|Int32|唯一的活动用户总数。 必填。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantUsage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantUsage",
  "id": "String (identifier)",
  "serviceUsages": [
    {
      "@odata.type": "microsoft.graph.managedTenants.serviceUsage"
    }
  ],
  "tenantId": "String",
  "reportDateTime": "String (timestamp)",
  "totalActiveUsers": "Integer"
}
```
