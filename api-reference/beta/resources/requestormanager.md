---
title: requestorManager 复杂类型
description: 标识与租户中将允许其成为审批者的另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4bfd42854a55ec2daa9e380c539a25479b0e933
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761077"
---
# <a name="requestormanager-complex-type"></a>requestorManager 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在访问包分配策略的 [审批设置中使用](accesspackageassignmentpolicy.md)。 它是 [userSet](userset.md)的子类型，其中值指示请求用户的经理 `@odata.type` `#microsoft.graph.requestorManager` 是审批者。  使用 requestorManager 创建访问包分配策略审批阶段时，还应包括另一个审批者，如单个用户或组的成员，以防请求的用户没有经理。


## <a name="properties"></a>属性


| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | 布尔 | 对于处于审批阶段的经理，指示该经理是否是备份回退审批者。 |
|managerLevel | Int32 | 请求者与经理的层次结构级别。 例如，请求者的直接经理的 managerLevel 为 1，而请求者经理的经理的 managerLevel 为 2。 managerLevel 的默认值为 1。 此属性的可能值范围为 1 到 2。 |


## <a name="json-representation"></a>JSON 表示形式

以下是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "managerLevel": 1
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


