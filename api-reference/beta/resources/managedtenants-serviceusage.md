---
title: serviceUsage 资源类型
description: 表示托管租户中服务的每月活动使用情况数据。
author: kylewirpel
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f680af26313e38da441408f6a127b21c14a7a045
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398948"
---
# <a name="serviceusage-resource-type"></a>serviceUsage 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户中服务的每月活动使用情况数据。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|monthlyActiveUsers|Int32|服务的每月活动用户数。 必填。 只读。|
|serviceName|String|生成使用情况的Microsoft 365服务的名称。 必填。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.serviceUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.serviceUsage",
  "serviceName": "String",
  "monthlyActiveUsers": "Integer"
}
```

