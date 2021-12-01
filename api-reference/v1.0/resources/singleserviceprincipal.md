---
title: singleServicePrincipal 复杂类型
description: 标识租户中将允许其作为请求者、审批者或审阅者的服务主体。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aaffcafdf0cc8f33efee350e15d0797ad5cba76e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242304"
---
# <a name="singleserviceprincipal-complex-type"></a>singleServicePrincipal 复杂类型

命名空间：microsoft.graph

在访问包分配策略的请求、审批和分配审阅设置中使用。 该值指示此 subjectSet 标识租户中将允许其成为请求者、审批者或审阅者 `@odata.type` `#microsoft.graph.singleServicePrincipal` 的特定服务主体。 [](../resources/subjectset.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|此服务主体的说明。|
|servicePrincipalId|String|[servicePrincipal 的](serviceprincipal.md)ID。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.singleServicePrincipal",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.singleServicePrincipal",
  "servicePrincipalId": "String",
  "description": "String"
}
```



