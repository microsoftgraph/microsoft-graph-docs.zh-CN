---
title: requestorSettings 复杂类型
description: 用于 `requestorSettings` 访问包分配策略的属性。 提供其他设置，以选择可以创建请求的人。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccaa57a3dfa2f81d33e4e6fea804a91d1db7da20
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777608"
---
# <a name="requestorsettings-resource-type"></a>requestorSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于访问 **包分配策略的 requestorSettings** [属性](accesspackageassignmentpolicy.md)。 提供其他设置，以选择可以在该策略上创建访问包请求的人。

| 谁可以请求 | scopeType | allowedRequestors 集合|
|:----------------|:----------|:------------------|
|没人|`NoSubjects`|空数组|
|目录中的特定单个用户|`SpecificDirectorySubjects`|[singleUser](singleuser.md)|
|目录中作为组成员的用户|`SpecificDirectorySubjects`|[groupMembers](groupmembers.md)|
|目录中值为 `userType``member`|`AllExistingDirectoryMemberUsers`|空数组|
|目录中的用户|`AllExistingDirectorySubjects`|空数组|
|特定连接组织中用户|`SpecificConnectedOrganizationSubjects`|[connectedOrganizationMembers](connectedorganizationmembers.md)|
|已连接组织的状态属性设置为的任何已连接组织的用户 `configured` 。|`AllConfiguredConnectedOrganizationSubjects`|空数组|
|任何用户|`AllExternalSubjects`|空数组|

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| scopeType |String |谁可以请求。 、 `NoSubjects` `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllConfiguredConnectedOrganizationSubjects` 或 `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` `AllExternalSubjects` 。  |
| acceptRequests | 布尔值 | 指示此策略是否接受新请求。 |
| allowedRequestors | [userSet](userset.md) 集合| 允许在此策略上请求的用户，可以是[singleUser、groupMembers](groupmembers.md)和[connectedOrganizationMembers。](connectedorganizationmembers.md) [](singleuser.md) |

## <a name="json-representation"></a>JSON 表示形式


下面是策略 **的 requestorSettings** 属性的 JSON 表示形式，允许组的成员进行请求。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings"
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


