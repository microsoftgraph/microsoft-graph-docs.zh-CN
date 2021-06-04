---
title: 用户资源类型
description: 表示 Azure Active Directory 用户对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f486e3202535882d719e5f6c083b583321e917b5
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732385"
---
# <a name="user-resource-type"></a>用户资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Azure Active Directory 用户对象。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 users](../api/intune-shared-user-list.md) 对象。|[user](../resources/intune-shared-user.md) 集合|列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。|
|[获取 user](../api/intune-shared-user-get.md) 对象。|[user](../resources/intune-shared-user.md) 集合|读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。|
|[创建 user](../api/intune-shared-user-create.md) 对象。|[user](../resources/intune-shared-user.md) 集合|创建新的 [user](../resources/intune-shared-user.md) 对象。|
|[删除用户](../api/intune-shared-user-delete.md)。|无|删除 [user](../resources/intune-shared-user.md)。|
|[更新 user](../api/intune-shared-user-update.md) 对象。|[user](../resources/intune-shared-user.md)|更新 [user](../resources/intune-shared-user.md) 对象的属性。|
|**设备管理**|
|[removeAllDevicesFromManagement 操作](../api/intune-shared-user-removealldevicesfrommanagement.md)|无|停用该用户管理的所有设备|
|**移动应用管理(MAM)**|
|[getManagedAppDiagnosticStatuses 函数](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合|获取给定用户的诊断验证状态。|
|[getManagedAppPolicies 函数](../api/intune-shared-user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|获取给定用户的应用限制。|
|[wipeManagedAppRegistrationsByDeviceTag 操作](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|无|对含有指定设备标记的应用注册发布擦除操作。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户的唯一标识符。|
|**载入**|
|deviceEnrollmentLimit|Int32|允许用户注册的最大设备数的限制。 允许的值为 5 或 1000。|


## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|**设备管理**|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) 集合|与用户关联的管理设备。|
|**移动应用管理(MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合|属于用户的零个或多个托管的应用注册。|
|**疑难解答**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合|此用户的故障排除事件列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
--> 
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->






