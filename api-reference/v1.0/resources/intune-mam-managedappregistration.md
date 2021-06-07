---
title: managedAppRegistration 资源类型
description: ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。 ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8eff848b54d3a84f6fb60d2c8335d71417f2afb0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755754"
---
# <a name="managedappregistration-resource-type"></a>managedAppRegistration 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。
ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
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
|flaggedReasons|[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) 集合|标记应用注册的零个或多个原因。 例如， 在取得 root 权限的设备上运行的应用|
|userId|String|此应用注册所属的用户 ID。|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|应用包标识符|
|id|String|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
|关系|类型|Description|
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




