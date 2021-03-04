---
title: riskyUserHistoryItem 资源类型
description: 表示 Azure AD 用户的风险历史记录
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4ae6d5fbc28e8dddb4c782aa9e9b2fad79b347ad
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442851"
---
# <a name="riskyuserhistoryitem-resource-type"></a>riskyUserHistoryItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
表示 Azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。 

## <a name="methods"></a>Methods

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列表历史记录](../api/riskyuser-list-history.md) | [riskyUserHistoryItem](riskyuserhistoryitem.md) 集合|获取 Azure AD 用户的风险历史记录。|


## <a name="properties"></a>属性

| 属性       | 类型    | 描述 |
|:---------------|:--------|:------------|
| userId         | string  | 用户的 ID。 |
| initiatedBy    | bool    | 执行该操作的主角的 ID。 |
| 活动       | [riskUserActivity](riskuseractivity.md)| 与用户风险级别相关的活动更改。 | 

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


