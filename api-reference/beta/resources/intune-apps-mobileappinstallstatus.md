---
title: mobileAppInstallStatus 资源类型
description: 包含设备的移动应用程序安装状态的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e71ebce532cf53528439be34937395837549f39
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792424"
---
# <a name="mobileappinstallstatus-resource-type"></a>mobileAppInstallStatus 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备的移动应用程序安装状态的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合|列出[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性和关系。|
|[获取 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|读取[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性和关系。|
|[创建 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。|
|[删除 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-delete.md)|无|删除[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。|
|[更新 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceName|String|设备名称|
|deviceId|String|设备 ID|
|lastSyncDateTime|DateTimeOffset|上次同步日期时间|
|将 mobileappinstallstatusvalue|[resultantAppState](../resources/intune-shared-resultantappstate.md)|应用程序的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|installState|[resultantAppState](../resources/intune-shared-resultantappstate.md)|应用程序的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|应用程序的安装状态详细信息。 可能的值为`noAdditionalDetails`: `dependencyFailedToInstall`、 `dependencyWithRequirementsNotMet`、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`、、、、、、、、、、、、、、、、 `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|errorCode|Int32|安装或卸载失败的错误代码。|
|osVersion|String|OS 版本|
|osDescription|String|OS 说明|
|userName|String|设备用户名|
|userPrincipalName|String|用户主体名称|
|displayVersion|String|人工可读版本的应用程序|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|应用程序|[mobileApp](../resources/intune-apps-mobileapp.md)|指向移动应用程序的导航链接。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```





