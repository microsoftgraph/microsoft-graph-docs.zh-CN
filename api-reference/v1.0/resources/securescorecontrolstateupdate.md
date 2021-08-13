---
title: secureScoreControlStateUpdate 资源类型
description: 此资源包含由用户更新的控件状态历史记录 (控件状态包括 Default、Ignored、ThirdParty、Reviewed) 。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3268b5f537b8538173031b3367ff0e13d2873a906dfe01a5b6d6562070812d56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146361"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型

命名空间：microsoft.graph

包含由用户更新的控件状态历史记录 (控件状态包括 Default、Ignored、ThirdParty、Reviewed) 。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|assignedTo|String|将控件分配给将执行该操作的用户。 |
|注释|String|提供有关控件的可选注释。 |
|state|String|控件的状态，可通过 PATCH 命令修改 (例如，忽略 thirdParty) 。 |
|updatedBy|String|更新租户状态的用户的 ID。 |
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

