---
title: externalSponsors 复杂类型
description: 标识与租户中将允许其成为审批者的另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 361ac6ff85d5b4462b39aa10e4f978ce7d486e40
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761868"
---
# <a name="externalsponsors-complex-type"></a>externalSponsors 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在访问包分配策略的 [审批阶段使用](accesspackageassignmentpolicy.md)。 它是 [userSet](userset.md)的子类型，其中值指示请求用户的已连接组织 `@odata.type` 外部发起 `#microsoft.graph.externalSponsors` 人将是审批者。 此审批者仅适用于来自已连接组织一部分的用户的请求。  使用 externalSponsors 创建访问包分配策略审批阶段时，还应包括另一个审批者，如单个用户或组的成员，以防连接的组织没有外部发起人。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | 布尔 | 指示发起人是否是备份回退审批者。 |

## <a name="json-representation"></a>JSON 表示形式

以下是此类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.externalSponsors",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


