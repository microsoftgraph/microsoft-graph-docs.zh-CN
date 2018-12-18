---
title: mobileAppAssignment 资源类型
description: 包含用于移动应用的组分配的属性的类。
author: tfitzmac
ms.openlocfilehash: 5f1413bc973d3721c7e9b01aa29e513028af9926
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320568"
---
# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





