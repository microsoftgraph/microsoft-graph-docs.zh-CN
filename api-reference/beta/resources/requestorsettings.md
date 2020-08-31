---
title: requestorSettings 复杂类型
description: 用于 `requestorSettings` 访问包分配策略的属性。 提供用于选择可以创建请求的何人的其他设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f54a0c00c7a906e67d8c2861eae7c8437a28fad0
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311835"
---
# <a name="requestorsettings-resource-type"></a>requestorSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于[访问包分配策略](accesspackageassignmentpolicy.md)的**requestorSettings**属性。 提供其他设置，以选择可在该策略上为访问包创建请求的成员。

| 谁可以请求 | scopeType | allowedRequestors 集合|
|:----------------|:----------|:------------------|
|没人|`NoSubjects`|空数组|
|目录中的特定个人用户|`SpecificDirectorySubjects`|[singleUser](singleuser.md)|
|目录中属于组成员的用户|`SpecificDirectorySubjects`|[groupMembers](groupmembers.md)|
|目录中 `userType` 值为的用户 `member`|`AllExistingDirectoryMemberUsers`|空数组|
|目录中的用户|`AllExistingDirectorySubjects`|空数组|
|特定连接组织中的用户|`SpecificConnectedOrganizationSubjects`|[connectedOrganizationMembers](connectedorganizationmembers.md)|
|将已连接组织的 state 属性设置为的任何已连接组织中的用户 `configured` 。|`AllConfiguredConnectedOrganizationSubjects`|空数组|
|任何用户|`AllExternalSubjects`|空数组|

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| scopeType |String |谁可以请求。 、、、、或中的一个 `NoSubjects` `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` `AllExternalSubjects` 。  |
| acceptRequests | Boolean | 指示是否在此策略上接受新的请求。 |
| allowedRequestors | [userSet](userset.md) 集合| 允许对此策略提出请求的用户，可以是 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)和 [connectedOrganizationMembers](connectedorganizationmembers.md)。 |

## <a name="json-representation"></a>JSON 表示形式


以下是策略的 **requestorSettings** 属性的 JSON 表示形式，它允许组的成员请求。

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
