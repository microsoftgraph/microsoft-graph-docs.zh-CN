---
title: windowsFeatureUpdateProfileAssignment 资源类型
description: 此实体包含用于将 windows 功能更新配置文件分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33808607c626196ac4627ea354da6f1f36e3f4ec
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199892"
---
# <a name="windowsfeatureupdateprofileassignment-resource-type"></a>windowsFeatureUpdateProfileAssignment 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体包含用于将 windows 功能更新配置文件分配给组的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsFeatureUpdateProfileAssignments](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-list.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)集合|列出[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性和关系。|
|[获取 windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-get.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|读取[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性和关系。|
|[创建 windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-create.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|创建新的[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象。|
|[删除 windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-delete.md)|无|删除[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)。|
|[更新 windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-update.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|更新[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的标识符|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|将功能更新配置文件分配到的工作分配目标。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



