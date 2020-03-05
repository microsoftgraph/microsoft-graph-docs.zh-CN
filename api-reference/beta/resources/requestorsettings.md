---
title: requestorSettings 复杂类型
description: 用于访问包`requestorSettings`分配策略的属性。 提供用于选择可以创建请求的何人的其他设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b52f3276185f819ccd0e7149dbd5420b4f6e1781
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521115"
---
# <a name="requestorsettings-resource-type"></a>requestorSettings 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于[访问包分配策略](accesspackageassignmentpolicy.md)的**requestorSettings**属性。 提供其他设置，以选择可在该策略上为访问包创建请求的成员。

| 谁可以请求 | scopeType | allowedRequestors 集合|
|:----------------|:----------|:------------------|
|没人|`NoSubjects`|空数组|
|目录中的特定个人用户|`SpecificDirectorySubjects`|[singleUser](singleuser.md)|
|目录中属于组成员的用户|`SpecificDirectorySubjects`|[groupMembers](groupmembers.md)|
|目录中`userType`值为的用户`member`|`AllExistingDirectoryMemberUsers`|空数组|
|目录中的用户|`AllExistingDirectorySubjects`|空数组|
|已配置特定其他连接组织中的用户|`SpecificConnectedOrganizationSubjects`|[connectedOrganizationMembers](connectedorganizationmembers.md)|
|已配置的任何其他已连接组织的用户|`AllExistingConnectedOrganizationSubjects`|空数组|
|任何用户|`AllExternalSubjects`|空数组|

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| scopeType |String |谁可以请求。 、、 `NoSubjects`、 `SpecificDirectorySubjects`、 `SpecificConnectedOrganizationSubjects` `AllExistingDirectorySubjects`或`AllExistingConnectedOrganizationSubjects` `AllExternalSubjects`中`AllExistingDirectoryMemberUsers`的一个。  |
| acceptRequests | 布尔 | 指示是否在此策略上接受新的请求。 |
| allowedRequestors | [userSet](userset.md)集合| 允许对此策略提出请求的用户，可以是[singleUser](singleuser.md)、 [groupMembers](groupmembers.md)和[connectedOrganizationMembers](connectedorganizationmembers.md)。 |

## <a name="json-representation"></a>JSON 表示形式


以下是策略的**requestorSettings**属性的 JSON 表示形式，它允许组的成员请求。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings",
  "baseType": ""
}-->

```json
{
  "scopeType": "SpecificDirectorySubjects",
  "acceptRequests": true,
  "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.groupMembers",
         "isBackup": false,
         "id": "string (identifier)",
         "description": "Authorized requestors"
       }
   ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
