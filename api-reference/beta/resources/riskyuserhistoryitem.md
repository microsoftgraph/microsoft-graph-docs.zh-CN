---
title: riskyUserHistoryItem 资源类型
description: 表示 Azure AD 用户的风险历史记录
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37f38a649aa3721e65b44e64571dafb797259cf6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620834"
---
# <a name="riskyuserhistoryitem-resource-type"></a>riskyUserHistoryItem 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
表示 azure AD 用户的风险历史记录, 由 Azure AD Identity Protection 确定。 

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
