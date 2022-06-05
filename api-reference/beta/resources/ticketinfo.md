---
title: ticketInfo 资源类型
description: 表示与角色分配和资格请求相关的票证信息。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e2356ef6fdbf0d1832d79fc2b68ecbef69db1ede
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900462"
---
# <a name="ticketinfo-resource-type"></a>ticketInfo 资源类型

命名空间：microsoft.graph

表示与角色分配和资格请求相关的票证信息。 使用此对象可以定义角色分配的票证参数，或者资格请求是由外部系统中发出的另一个请求发起的。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ticketNumber|字符串|票证号。|
|ticketSystem|字符串|票证系统的说明。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ticketInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ticketInfo",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

