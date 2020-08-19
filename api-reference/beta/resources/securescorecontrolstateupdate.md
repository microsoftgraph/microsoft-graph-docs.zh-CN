---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含由用户更新的控制状态的历史记录 (控制状态包括默认、已忽略、ThirdParty、已审阅) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f3b69838a6de68938efac12acdfbcd4fd977c684
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810403"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型
包含用户更新的控件状态的历史记录 (控件状态包括默认值、被忽略的 ThirdParty、已审阅的) 。

|属性 |类型 |说明 |
|:--|:--|:--|
|assignedTo | string | 将控件分配给将执行该操作的用户 |
|comment | string | 提供有关控件的可选注释 |
|state | string | 可以使用 PATCH 命令修改控件的状态 (Ex：忽略、thirdParty 等)  |
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
