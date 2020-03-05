---
title: externalSponsors 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03e73fe63e7624b2ab9d549c3b9ccd1526301a9c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498607"
---
# <a name="externalsponsors-complex-type"></a>externalSponsors 复杂类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[访问包分配策略](accesspackageassignmentpolicy.md)的审批阶段中使用。 它是[userSet](userset.md)的一个子类型，其中`@odata.type`值`#microsoft.graph.externalSponsors`表示请求用户的已连接组织的外部发起人是审批者。 此审批者仅适用于来自属于已连接组织的用户的请求。  在使用 externalSponsors 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防所连接的组织没有外部发起人。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | 布尔 | 指示发起人是否为备份回退审批者。 |

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
