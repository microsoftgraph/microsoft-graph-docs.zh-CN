---
title: riskyUserHistoryItem 资源类型
description: 表示Azure AD用户的风险历史记录
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6a415325c26226ad2400ce572146bbfaa5beb8c7
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060666"
---
# <a name="riskyuserhistoryitem-resource-type"></a>riskyUserHistoryItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
表示由Azure AD标识保护确定的Azure AD用户的风险历史记录。

>[!NOTE]
> 1. 使用此 API 需要Azure AD Premium P2许可证。
> 2. 风险历史记录数据的可用性受[Azure AD数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)的控制。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出历史记录](../api/riskyuser-list-history.md) | [riskyUserHistoryItem](riskyuserhistoryitem.md) 集合|获取Azure AD用户的风险历史记录。|


## <a name="properties"></a>属性

| 属性       | 类型    | 描述 |
|:---------------|:--------|:------------|
| userId         | string  | 用户的 ID。 |
| initiatedBy    | 布尔值    | 执行操作的执行组件的 ID。 |
| 活动       | [riskUserActivity](riskuseractivity.md)| 与用户风险级别更改相关的活动。 | 

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


