---
title: deviceAppManagement 资源类型
description: 设备应用管理单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8906e96a0218360bbe78d1c08dd4d8767568775
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751839"
---
# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备应用管理单例实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedAppPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|托管应用策略。|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 集合|iOS 托管应用策略。|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 集合|Android 托管应用策略。|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 集合|默认的托管应用策略。|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合|托管应用配置目标。|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 集合|对已注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 集合|对未注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合|托管应用注册。|
|managedAppStatuses|[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合|托管应用状态。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




