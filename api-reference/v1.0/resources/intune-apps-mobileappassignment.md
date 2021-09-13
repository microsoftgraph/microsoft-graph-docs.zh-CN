---
title: mobileAppAssignment 资源类型
description: 包含用于移动应用的组分配的属性的类。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b8a635684ea6010bef8eabe7a5244d20024d4389
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123207"
---
# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "String"
  }
}
```




