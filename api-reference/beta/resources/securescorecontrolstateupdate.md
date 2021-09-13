---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含由用户更新的控件 (状态，包括 Default、Ignored、ThirdParty、Reviewed) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 17d35370907ac82d47b28e67b7fb4ba6c0068bb7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063613"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型
包含由用户更新的控件状态历史记录 (控件状态包括 Default、Ignored、ThirdParty、Reviewed) 。

|属性 |类型 |说明 |
|:--|:--|:--|
|assignedTo | 字符串 | 将控件分配给将采取措施的用户 |
|comment | string | 提供有关控件的可选注释 |
|state | string | 可以使用 PATCH 命令修改控件的状态，例如 (、thirdParty 等)  |
|updatedBy | 字符串 |更新租户状态的用户的 ID |
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


