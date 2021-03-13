---
title: internalSponsors 复杂类型
description: 标识与租户中将允许其成为审批者的另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84c53bbeacde51afc88f5c0b4b5c13bc4f68b430
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760895"
---
# <a name="internalsponsors-complex-type"></a>internalSponsors 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在访问包分配策略的 [审批阶段使用](accesspackageassignmentpolicy.md)。 它是 [userSet](userset.md)的子类型，其中值指示请求用户的已连接组织内部发起 `@odata.type` `#microsoft.graph.internalSponsors` 人将是审批者。 此审批者仅适用于来自已连接组织一部分的用户的请求。  使用 internalSponsors 创建访问包分配策略审批阶段时，还应包括另一个审批者，例如单个用户或组的成员，以防连接的组织没有内部发起人。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | 布尔 | 指示发起人是否是备份回退审批者。 |

## <a name="json-representation"></a>JSON 表示形式

以下是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.internalSponsors",
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


