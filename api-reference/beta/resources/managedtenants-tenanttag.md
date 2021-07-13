---
title: tenantTag 资源类型
description: 表示可分配给托管租户的标记。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e48ad25e2af3ac491c6affe4bbb4712ab45e42fc
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402245"
---
# <a name="tenanttag-resource-type"></a>tenantTag 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可分配给托管租户的标记。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 tenantTags](../api/managedtenants-managedtenant-list-tenanttags.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md) 集合|获取 [tenantTag 对象](../resources/managedtenants-tenanttag.md) 及其属性的列表。|
|[创建 tenantTag](../api/managedtenants-managedtenant-post-tenanttags.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|创建新的 [tenantTag](../resources/managedtenants-tenanttag.md) 对象。|
|[获取 tenantTag](../api/managedtenants-tenanttag-get.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|读取 [tenantTag](../resources/managedtenants-tenanttag.md) 对象的属性和关系。|
|[更新 tenantTag](../api/managedtenants-tenanttag-update.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|更新 [tenantTag 对象](../resources/managedtenants-tenanttag.md) 的属性。|
|[删除 tenantTag](../api/managedtenants-tenanttag-delete.md)|无|删除 [tenantTag](../resources/managedtenants-tenanttag.md) 对象。|
|[assignTag](../api/managedtenants-tenanttag-assigntag.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|将租户标记分配给指定的托管租户。|
|[unassignTag](../api/managedtenants-tenanttag-unassigntag.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|从指定的托管租户中取消分配租户标记。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdByUserId|String|创建租户标记的帐户的标识符。 必填。 只读。|
|createdDateTime|DateTimeOffset|创建租户标记的日期和时间。 必填。 只读。|
|deletedDateTime|DateTimeOffset|删除租户标记的日期和时间。 必填。 只读。|
|说明|String|租户标记的说明。 可选。 只读。|
|displayName|String|租户显示名称的变量。 必填。 只读。|
|id|String|租户标记的唯一标识符。 必填。 只读。|
|lastActionByUserId|String|持续在租户标记上的帐户的标识符。 可选。 只读。|
|lastActionDateTime|DateTimeOffset|上次对租户标记执行的操作的日期和时间。 可选。 只读。|
|tenants|[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) 集合|与租户标记关联的托管租户的集合。 可选。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantTag",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdByUserId": "String",
  "lastActionByUserId": "String",
  "tenants": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
    }
  ],
  "lastActionDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)"
}
```
