---
title: riskyServicePrincipalHistoryItem 资源类型
description: 表示服务主体Azure AD历史记录
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aaafd1236a31530c32ca9cb6f62db932a0588f9e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519933"
---
# <a name="riskyserviceprincipalhistoryitem-resource-type"></a>riskyServicePrincipalHistoryItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
表示由 Identity Protection 确定Azure AD服务主体Azure AD历史记录。 继承自 [riskyServicePrincipal](riskyserviceprincipal.md)。

## <a name="methods"></a>Methods

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列表历史记录](../api/riskyserviceprincipal-list-history.md) | [riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md) 集合|获取服务主体Azure AD历史记录。|


## <a name="properties"></a>属性

| 属性       | 类型    | 说明 |
|:---------------|:--------|:------------|
| servicePrincipalId         | 字符串  | 服务主体的标识符。 |
| initiatedBy    | 布尔值    | 操作执行者标识符。 |
| 活动       | [riskServicePrincipalActivity](riskserviceprincipalactivity.md)| 与服务主体风险级别相关的活动会发生变化。 | 

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyServicePrincipalHistoryItem",
  "baseType": "microsoft.graph.riskyServicePrincipal"
}-->

```json
{
    "servicePrincipalId": "String",
    "initiatedBy": "String",
    "activity": {"@odata.type": "microsoft.graph.riskServicePrincipalActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyServicePrincipalHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
