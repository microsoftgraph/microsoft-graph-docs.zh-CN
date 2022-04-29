---
title: ticketInfo 资源类型
description: 表示与角色分配和资格请求相关的票证信息。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e2356ef6fdbf0d1832d79fc2b68ecbef69db1ede
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133919"
---
# <a name="ticketinfo-resource-type"></a>ticketInfo 资源类型

命名空间：microsoft.graph

表示与角色分配和资格请求相关的票证信息。 使用此对象可以定义角色分配的票证参数，或者资格请求是由外部系统中发出的另一个请求发起的。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ticketNumber|String|票证号。|
|ticketSystem|String|票证系统的说明。|

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

