---
title: policySetAssignment 资源类型
description: 一个包含用于 PolicySet Assignment 的属性的类。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a19e310f89742b14b9c1d12f1d69725b0b699aa0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074869"
---
# <a name="policysetassignment-resource-type"></a>policySetAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个包含用于 PolicySet Assignment 的属性的类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 policySetAssignments](../api/intune-policyset-policysetassignment-list.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md) 集合|列出 [policySetAssignment](../resources/intune-policyset-policysetassignment.md) 对象的属性和关系。|
|[获取 policySetAssignment](../api/intune-policyset-policysetassignment-get.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|读取 [policySetAssignment](../resources/intune-policyset-policysetassignment.md) 对象的属性和关系。|
|[创建 policySetAssignment](../api/intune-policyset-policysetassignment-create.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|创建新的 [policySetAssignment](../resources/intune-policyset-policysetassignment.md) 对象。|
|[删除 policySetAssignment](../api/intune-policyset-policysetassignment-delete.md)|无|删除 [policySetAssignment](../resources/intune-policyset-policysetassignment.md)。|
|[更新 policySetAssignment](../api/intune-policyset-policysetassignment-update.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|更新 [policySetAssignment 对象](../resources/intune-policyset-policysetassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|PolicySetAssignment 的键。|
|lastModifiedDateTime|DateTimeOffset|PolicySetAssignment 的上次修改时间。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|PolicySetAssignment 的目标组|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```



