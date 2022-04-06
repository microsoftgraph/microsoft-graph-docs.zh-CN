---
title: accessPackageAssignmentRequestorSettings 资源类型
description: 用于访问包分配策略的 requestorSettings 属性。 提供其他设置，以选择可以创建请求的人。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d7a60166f60c2c5882872ed011722fbe14257462
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608284"
---
# <a name="accesspackageassignmentrequestorsettings-complex-type"></a>accessPackageAssignmentRequestorSettings 复杂类型

命名空间：microsoft.graph

用于访问包分配策略 [的请求者设置](accesspackageassignmentpolicy.md)。 提供其他设置，以选择可以在该策略上创建访问包请求的人，以及可以在请求中包括的内容。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|allowCustomAssignmentSchedule|Boolean|如果 `false`为 ，则不允许请求者在请求中包括计划。|
|enableOnBehalfRequestorsToAddAccess|布尔|如果 `true`为 ，则允许代表请求者创建请求，以添加其他主体的访问权限。|
|enableOnBehalfRequestorsToRemoveAccess|Boolean|如果 `true`为 ，则允许代表请求者创建删除其他主体的访问权限的请求。|
|enableOnBehalfRequestorsToUpdateAccess|Boolean|如果 `true`为 ，则允许代表请求者创建请求以更新其他主体的访问。|
|enableTargetsToSelfAddAccess|Boolean|如果 `true`为 ，则允许请求者创建请求，以为自己添加访问权限。|
|enableTargetsToSelfRemoveAccess|Boolean|如果 `true`为 ，则允许请求者创建删除其访问权限的请求。|
|enableTargetsToSelfUpdateAccess|布尔|如果 `true`为 ，则允许请求者创建请求以更新其访问权限。|
|onBehalfRequestors|[subjectSet](../resources/subjectset.md) 集合|可以代表他人请求的主体。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestorSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestorSettings",
  "enableTargetsToSelfAddAccess": "Boolean",
  "enableTargetsToSelfUpdateAccess": "Boolean",
  "enableTargetsToSelfRemoveAccess": "Boolean",
  "allowCustomAssignmentSchedule": "Boolean",
  "enableOnBehalfRequestorsToAddAccess": "Boolean",
  "enableOnBehalfRequestorsToUpdateAccess": "Boolean",
  "enableOnBehalfRequestorsToRemoveAccess": "Boolean",
  "onBehalfRequestors": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```


