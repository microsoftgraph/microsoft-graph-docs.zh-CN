---
title: secureScoreControlStateUpdate 资源类型
description: 此资源包含用户更新的控件状态的历史记录（控件状态包括默认、忽略、ThirdParty、已审阅）。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0fe88741da75718b1509fd4f8015a37fcf7828bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446959"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型

命名空间： microsoft. graph

包含用户更新的控件状态的历史记录（控件状态包括默认、忽略、ThirdParty、已审阅）。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|assignedTo|String|将控件分配给将执行该操作的用户。 |
|注释|String|提供有关控件的可选注释。 |
|state|String|控件的状态，可通过修补程序命令进行修改（例如，忽略、thirdParty）。 |
|updatedBy|String|更新了租户状态的用户的 ID。 |
|updatedDateTime|DateTimeOffset|控件状态的更新时间。 |

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
