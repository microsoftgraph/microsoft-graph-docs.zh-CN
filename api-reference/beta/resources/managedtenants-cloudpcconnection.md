---
title: cloudPcConnection 资源类型
description: 表示给定托管租户的云电脑连接。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f7f306a54354d0c6d4860abd0866001f5e8626f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860430"
---
# <a name="cloudpcconnection-resource-type"></a>cloudPcConnection 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管租户的云电脑连接。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPcConnections](../api/managedtenants-managedtenant-list-cloudpcconnections.md)|[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 集合|获取 [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 对象及其属性的列表。|
|[获取 cloudPcConnection](../api/managedtenants-cloudpcconnection-get.md)|[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|读取 [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|云显示名称连接类型。 必需。 只读。|
|healthCheckStatus|String|云电脑连接的运行状况。 可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。  必需。 只读。|
|id|String|云电脑连接的唯一标识符。 必需。 只读。|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 必需。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 必需。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 必需。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcConnection",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "healthCheckStatus": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
