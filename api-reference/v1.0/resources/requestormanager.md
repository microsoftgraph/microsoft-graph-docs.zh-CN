---
title: requestorManager 复杂类型
description: 标识与租户中将允许其成为审批者的另一个用户的关系。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a4f82b55438fe2e077cca299d55aa6af2c0fecb
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242398"
---
# <a name="requestormanager-complex-type"></a>requestorManager 复杂类型

命名空间：microsoft.graph

在访问包分配策略的审批设置中使用。
它是 [subjectSet](subjectset.md)的子类型，其中值指示请求用户的经理是 `@odata.type` `#microsoft.graph.requestorManager` 审批者。  使用 requestorManager 创建访问包分配策略审批阶段时，还应包括另一个审批者，如单个用户或组的成员，以防请求的用户没有经理。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|managerLevel|Int32|请求者与经理的层次结构级别。 例如，请求者的直接经理的 managerLevel 为 1，而请求者经理的经理的 managerLevel 为 2。 managerLevel 的默认值为 1。 此属性的可能值范围为 1 到 2。 |

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestorManager",
  "managerLevel": "Integer"
}
```


