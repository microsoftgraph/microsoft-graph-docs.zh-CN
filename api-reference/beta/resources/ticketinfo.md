---
title: ticketInfo 资源类型
description: 表示与请求相关的票证角色分配的对象
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2d97d4f220a4579b805959c3b5d9c369293b2730
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453637"
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

