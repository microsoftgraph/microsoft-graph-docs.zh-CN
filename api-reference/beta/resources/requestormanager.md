---
title: requestorManager 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b2e3062383dd1cc1c7d04342b2dcbd5be0afd67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521122"
---
# <a name="requestomanager-complex-type"></a>requestoManager 复杂类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[访问包分配策略](accesspackageassignmentpolicy.md)的审批设置中使用。 它是[userSet](userset.md)的子类型，其中`@odata.type`值`#microsoft.graph.requestorManager`表示请求用户的经理是审批者。  在使用 requestorManager 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防请求用户没有经理。


## <a name="properties"></a>属性


| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | 布尔 | 对于审批阶段中的经理，指示管理器是否为备份回退审批者。 |

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
  "isBackup": false
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
