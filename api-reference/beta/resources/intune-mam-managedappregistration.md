---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a343dba3df1274693449b8f7cbefd83b131138c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421436"
---
# <a name="managedappregistration-resource-type"></a>managedAppRegistration 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。
ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAppRegistrations](../api/intune-mam-managedappregistration-list.md)|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合|列出 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。|
|[Get managedAppRegistration](../api/intune-mam-managedappregistration-get.md)|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)|读取 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) 对象的属性和关系。|
|[getUserIdsWithFlaggedAppRegistration 函数](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|String collection|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建日期和时间|
|lastSyncDateTime|DateTimeOffset|上次应用与管理服务同步的日期和时间。|
|applicationVersion|String|应用版本|
|managementSdkVersion|String|应用管理 SDK 版本|
|platformVersion|String|操作系统版本|
|deviceType|String|主机设备类型|
|deviceTag|String|应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。 不保证在所有情况下与应用关联。|
|deviceName|String|主机设备名称|
|managedDeviceId|String|主机设备管理的设备标识符。 即使托管主机设备，则可能为空值。|
|azureADDeviceId|String|主机设备 Azure Active Directory 设备标识符。 即使主机设备注册的 Azure Active Directory，值可能为空。|
|deviceModel|String|当前应用程序注册设备模型 |
|deviceManufacturer|String|设备制造商的当前应用程序注册 |
|flaggedReasons|[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)集合|标记应用注册的零个或多个原因。 例如， 在取得 root 权限的设备上运行的应用|
|userId|String|此应用注册所属的用户 ID。|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|应用包标识符|
|id|String|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。|
|intendedPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|目前适用于应用的零个或多个策略管理员。|
|操作|[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合|在应用注册时触发的零个或多个长时间运行的操作。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




