---
title: ticketInfo 资源类型
description: 表示与请求相关的票证角色分配的对象
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 410b978184efdc098dfa05c08717d7ca471ffe9c
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64508466"
---
# <a name="ticketinfo-resource-type"></a>ticketInfo 资源类型

命名空间：microsoft.graph

表示与请求相关的票证角色分配的对象

## <a name="properties"></a>属性
|属性|类型|说明|
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

