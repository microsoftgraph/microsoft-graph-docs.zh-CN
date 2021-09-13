---
title: ticketInfo 资源类型
description: 表示与请求相关的票证角色分配的对象
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b3a330071fa6d17ff510901376d1fb3b0c1c0cdb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023113"
---
# <a name="ticketinfo-resource-type"></a>ticketInfo 资源类型

命名空间：microsoft.graph

表示与请求相关的票证角色分配的对象

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|ticketNumber|String|票证编号元数据|
|ticketSystem|String|票证系统元数据|

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

