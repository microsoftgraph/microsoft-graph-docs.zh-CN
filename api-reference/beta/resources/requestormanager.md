---
title: requestorManager 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca8559d3ecf7ba4110a7e2871f8e6acf545d2906
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581150"
---
# <a name="requestormanager-complex-type"></a>requestorManager 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [访问包分配策略](accesspackageassignmentpolicy.md)的审批设置中使用。 它是 [userSet](userset.md)的子类型，其中 `@odata.type` 值 `#microsoft.graph.requestorManager` 表示请求用户的经理是审批者。  在使用 requestorManager 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防请求用户没有经理。


## <a name="properties"></a>属性


| 属性                     | 类型                      | Description |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | 布尔值 | 对于审批阶段中的经理，指示管理器是否为备份回退审批者。 |
|managerLevel | Int32 | 经理相对于请求者的层次结构级别。 例如，请求者的直接经理的 managerLevel 为1，而请求者的经理的经理的 managerLevel 为2。 ManagerLevel 的默认值为1。 此属性的可能值范围为1到2。 |


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


