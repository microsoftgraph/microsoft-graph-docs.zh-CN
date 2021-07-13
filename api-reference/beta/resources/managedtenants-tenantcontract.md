---
title: tenantContract 资源类型
description: 表示租户和管理实体之间的关系信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 104b475428efe82a2e56f823845b933149aeab18
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402276"
---
# <a name="tenantcontract-resource-type"></a>tenantContract 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户和管理实体之间的关系信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contractType|Int32|管理实体和租户之间存在的关系类型。 可选。 只读。|
|defaultDomainName|String|租户的默认域名。 必填。 只读。|
|displayName|String|租户的显示名称。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContract"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContract",
  "contractType": "Integer",
  "displayName": "String",
  "defaultDomainName": "String"
}
```
