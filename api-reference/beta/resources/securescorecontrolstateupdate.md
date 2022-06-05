---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含用户更新的控件状态的历史记录 (控制状态包括 Default、Ignored、ThirdParty、Reviewed) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 72be4693fa6b851ee587462d96451d78430a24a6
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899509"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型
包含用户更新的控件状态的历史记录 (控件状态包括 Default、Ignored、ThirdParty、Reviewed) 。

|属性 |类型 |说明 |
|:--|:--|:--|
|assignedTo | string | 将控件分配给将执行该操作的用户 |
|comment | string | 提供有关控件的可选注释 |
|state | string | 可以使用 PATCH 命令修改控件的状态 (Ex：ignored、thirdParty 等)  |
|updatedBy | string |更新租户状态的用户的 ID |
|updatedDateTime | DateTimeOffset |更新控制状态的时间 |
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


