---
title: targetManager 资源类型
description: 指示经理（包括用户的间接经理）可能代表该用户请求的权利管理的复杂类型。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 06859aea4cc966ca25ded6dc8e972adf6ca2a600
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608291"
---
# <a name="targetmanager-complex-type"></a>targetManager 复杂类型

命名空间：microsoft.graph

在访问包分配策略中，此类型继承自 [subjectSet](../resources/subjectset.md) ，并指示经理（包括用户的间接经理）可以代表该用户请求。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|managerLevel|Int32|经理级别，介于 1 和 4 之间。 直接经理为 1。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.targetManager"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetManager",
  "managerLevel": "Integer"
}
```


