---
title: intuneBrandingProfileAssignment 资源类型
description: 此实体包含用于向组分配品牌配置文件的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99d5aa43eb52e4ad12b34c231c953ccaa23d89a4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153590"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>intuneBrandingProfileAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体包含用于向组分配品牌配置文件的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 intuneBrandingProfileAssignments](../api/intune-wip-intunebrandingprofileassignment-list.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) 集合|列出 [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) 对象的属性和关系。|
|[获取 intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|读取 [intuneBrandingProfileAssignment 对象的属性和](../resources/intune-wip-intunebrandingprofileassignment.md) 关系。|
|[创建 intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|创建新的 [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) 对象。|
|[删除 intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-delete.md)|无|删除 [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)。|
|[更新 intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|更新 [intuneBrandingProfileAssignment 对象](../resources/intune-wip-intunebrandingprofileassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一标识符。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|品牌配置文件分配到的分配目标。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




