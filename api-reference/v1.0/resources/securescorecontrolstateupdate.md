---
title: secureScoreControlStateUpdate 资源类型
description: 此资源包含用户更新的控件状态的历史记录 (控件状态包括 Default、Ignored、ThirdParty、Reviewed) 。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5c91abead33b725862242e2f8864371729668583
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898894"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型

命名空间：microsoft.graph

包含用户更新的控件状态的历史记录 (控件状态包括 Default、Ignored、ThirdParty、Reviewed) 。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|assignedTo|String|将控件分配给将执行该操作的用户。 |
|注释|String|提供有关控件的可选注释。 |
|state|String|控件的状态，可通过 PATCH 命令进行修改 (例如忽略，第三部分) 。 |
|updatedBy|字符串|更新租户状态的用户的 ID。 |
|updatedDateTime|DateTimeOffset|更新控件状态的时间。 |

## <a name="json-representation"></a>JSON 表示形式
 下面是资源的 JSON 表示形式。
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
    
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "String (timestamp)"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

