---
title: eventQuery 资源类型
description: 表示与保留事件关联的工作负荷 (SharePoint Online、OneDrive for Business、Exchange Online) 和标识信息。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: bfdb65f2609947b6cc820c5c4937925c5b340115
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447599"
---
# <a name="eventquery-resource-type"></a>eventQuery 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与保留事件关联的工作负荷 (SharePoint Online、OneDrive for Business、Exchange Online) 和标识信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|queryType|microsoft.graph.security.queryType|表示与事件关联的查询类型。 SPO 和 ODB 的“文件”和 EXO 的“消息”。可能的值为： `files`， ， `messages`。 `unknownFutureValue`|
|查询|String|表示查询的唯一标识。 SharePoint Online 和 OneDrive for Business 的“资产 ID”，Exchange Online的“关键字”。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.eventQueries"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.eventQuery",
  "queryType": "String",
  "query": "String"
}
```


