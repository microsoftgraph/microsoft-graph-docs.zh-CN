---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含用户更新的控制状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549137"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型
包含用户更新的控件状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。

|属性 |类型 |说明 |
|:--|:--|:--|
|assignedTo | string | 将控件分配给将执行该操作的用户 |
|comment | string | 提供有关控件的可选注释 |
|state | string | 可以使用 "修补程序" 命令修改控件的状态 (Ex: 忽略、thirdParty 等) |
|updatedBy | string |更新了租户状态的用户的 ID |
|updatedDateTime | DateTimeOffset? |更新控件状态的时间 |
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
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
