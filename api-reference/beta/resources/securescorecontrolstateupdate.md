---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含控件状态更新的用户的历史记录 （控件状态包括默认、 忽略、 ThirdParty、 已审阅）。
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574388"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含由用户更新控件状态的历史记录 （控件状态包括默认、 忽略、 ThirdParty、 已审阅）。

|属性         | 类型           |说明                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| assignedTo      | string         | 分配将执行的操作的用户控件     |
| 批注         | string         | 提供有关控件的可选注释                 |
| state           | string         | 可以使用修补程序命令修改控件的状态 (例如： 忽略，第三方等) |
| updatedBy       | string         |更新租户状态的用户的 ID                      |
| updatedDateTime | DateTimeOffset |在哪个控件更新状态的时间                      |
 

## <a name="json-representation"></a>JSON 表示形式
 下面是资源的 JSON 表示形式。

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
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
