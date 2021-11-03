---
title: ticketInfo 资源类型
description: 表示与请求相关的票证角色分配的对象
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e75cd3f594a515e83abb59d0b476e4d130771875
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694902"
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

