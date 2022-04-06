---
title: accessPackageAssignmentApprovalSettings 复杂类型
description: 指定在访问包分配策略中审批访问包分配请求的设置。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5109cdd2482c43188409f891f782179bc1a39ebb
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608293"
---
# <a name="accesspackageassignmentapprovalsettings-complex-type"></a>accessPackageAssignmentApprovalSettings 复杂类型

命名空间：microsoft.graph

用于访问 **包分配策略的 requestApprovalSettings** [属性](accesspackageassignmentpolicy.md)。 提供其他设置，以指示是否通过该策略对访问包分配的新请求或对现有请求的更新进行审批，以及选择必须批准每个请求的人。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|isApprovalRequiredForAdd|Boolean|如果 `false,` 此策略中的新请求不需要审批，|
|isApprovalRequiredForUpdate|布尔|如果 `false`为 ，则此策略中的请求更新不需要审批。|
|stages|[accessPackageApprovalStage](../resources/accesspackageapprovalstage.md) 集合|如果需要审批，则此集合的一个、两个或三个元素将定义审批的每个阶段。 如果不需要批准，则存在空数组。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentApprovalSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentApprovalSettings",
  "isApprovalRequiredForAdd": "Boolean",
  "isApprovalRequiredForUpdate": "Boolean",
  "stages": [
    {
      "@odata.type": "microsoft.graph.accessPackageApprovalStage"
    }
  ]
}
```


