---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含用户更新的控制状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92616569a87a6ccf91c17ea7c845b8185bd33e8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965227"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型
包含用户更新的控件状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。

|属性 |类型 |说明 |
|:--|:--|:--|
|assignedTo | string | 将控件分配给将执行该操作的用户 |
|comment | string | 提供有关控件的可选注释 |
|state | string | 可以使用 "修补程序" 命令修改控件的状态 (Ex: 忽略、thirdParty 等) |
|updatedBy | string |更新了租户状态的用户的 ID |
|updatedDateTime | DateTimeOffset |更新控件状态的时间 |
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
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
