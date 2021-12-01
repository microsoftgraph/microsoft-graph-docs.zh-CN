---
title: singleUser 复杂类型
description: 标识租户中将允许其成为请求者、审批者或审阅者的用户。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9cc5549ef34fb9ee67a3337e0ba40bc38f413469
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242378"
---
# <a name="singleuser-complex-type"></a>singleUser 复杂类型

命名空间：microsoft.graph

在访问包分配策略的请求、审批和分配审阅设置中使用。 该值指示此 userSet 标识租户中将允许其成为请求者、审批者或审阅者  `@odata.type` `#microsoft.graph.singleUser` 的特定用户。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|Azure AD。 只读。 |
|userId|String|Azure AD 中的用户[](user.md)ID。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.singleUser",
  "userId": "String",
  "description": "String"
}
```



