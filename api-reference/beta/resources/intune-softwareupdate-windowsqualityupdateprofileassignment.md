---
title: windowsQualityUpdateProfileAssignment 资源类型
description: 此实体包含用于向组分配 Windows 质量更新配置文件的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e42d5129bde3fc3df988eebac4712f15f9efe60
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162227"
---
# <a name="windowsqualityupdateprofileassignment-resource-type"></a>windowsQualityUpdateProfileAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体包含用于向组分配 Windows 质量更新配置文件的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsQualityUpdateProfileAssignments](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-list.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) 集合|列出 [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) 对象的属性和关系。|
|[获取 windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-get.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|读取 [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) 对象的属性和关系。|
|[创建 windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-create.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|创建新的 [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) 对象。|
|[删除 windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-delete.md)|无|删除 [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)。|
|[更新 windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-update.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|更新 [windowsQualityUpdateProfileAssignment 对象](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的标识符|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|功能更新配置文件分配到的分配目标。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




