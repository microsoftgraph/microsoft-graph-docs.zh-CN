---
title: androidManagedAppRegistration 资源类型
description: 表示特定用户具有管理功能的 Android 应用的同步详细信息。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01465444f3cce6dba57cebb1c5827e05b78f4a2e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754970"
---
# <a name="androidmanagedappregistration-resource-type"></a>androidManagedAppRegistration 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示特定用户具有管理功能的 Android 应用的同步详细信息。
ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。


继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List androidManagedAppRegistrations](../api/intune-mam-androidmanagedappregistration-list.md)|[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 集合|列出 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。|
|[Get androidManagedAppRegistration](../api/intune-mam-androidmanagedappregistration-get.md)|[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md)|读取 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象的属性和关系。|
|[创建 androidManagedAppRegistration](../api/intune-mam-androidmanagedappregistration-create.md)|[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md)|创建新的 [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建的日期和时间。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|lastSyncDateTime|DateTimeOffset|上次应用与管理服务同步的日期和时间。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|applicationVersion|String|应用版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|managementSdkVersion|String|应用管理 SDK 版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|platformVersion|String|操作系统版本。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceType|String|主机设备类型。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceTag|String|应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。 不保证在所有情况下与应用关联。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceName|String|主机设备名称。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|flaggedReasons|[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合|标记应用注册的零个或多个原因。 例如， 应用正在根设备上运行 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|userId|String|此应用注册所属的用户 ID。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|应用包标识符。继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|id|String|实体的键。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|version|String|实体的版本。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|intendedPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|目前适用于应用的零个或多个策略管理员。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|operations|[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合|在应用注册时触发的零个或多个长时间运行的操作。 继承自 [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




