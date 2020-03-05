---
title: riskyUserHistoryItem 资源类型
description: 表示 Azure AD 用户的风险历史记录
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 519e2a7fdb6662496cdb660095ec63ce81b849f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521052"
---
# <a name="riskyuserhistoryitem-resource-type"></a>riskyUserHistoryItem 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
表示 azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。 

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列表历史记录](../api/riskyuser-list-history.md) | [riskyUserHistoryItem](riskyuserhistoryitem.md)集合|获取 Azure AD 用户的风险历史记录。|


## <a name="properties"></a>属性

| 属性       | 类型    | 说明 |
|:---------------|:--------|:------------|
| userId         | string  | 用户的 id。 |
| initiatedBy    | 布尔值    | 执行此操作的主角的 id。 |
| activity       | [riskUserActivity](riskuseractivity.md)| 与用户风险级别更改相关的活动。 | 

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
