---
title: mobileAppAssignment 资源类型
description: 包含用于移动应用的组分配的属性的类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec9901c8f07e2ae56500c1b99aac1fcce1bfb379
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404517"
---
# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于移动应用的组分配的属性的类。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppAssignments](../api/intune-apps-mobileappassignment-list.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|列出 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性和关系。|
|[获取 mobileAppAssignment](../api/intune-apps-mobileappassignment-get.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|读取 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性和关系。|
|[创建 mobileAppAssignment](../api/intune-apps-mobileappassignment-create.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。|
|[删除 mobileAppAssignment](../api/intune-apps-mobileappassignment-delete.md)|无|删除 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|
|[更新 mobileAppAssignment](../api/intune-apps-mobileappassignment-update.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|intent|[installIntent](../resources/intune-shared-installintent.md)|由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|由管理员定义的目标组分配。|
|settings|[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)|由管理员定义的目标分配的设置。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```




