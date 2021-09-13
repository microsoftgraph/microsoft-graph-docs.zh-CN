---
title: mobileAppInstallStatus 资源类型
description: 包含设备移动应用的安装状态的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0853dc6c2fb471dc6617f0a7bdef658ed284b5ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59087000"
---
# <a name="mobileappinstallstatus-resource-type"></a>mobileAppInstallStatus 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备移动应用的安装状态的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合|列出 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。|
|[获取 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|读取 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。|
|[创建 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|创建新的 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象。|
|[删除 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-delete.md)|无|删除 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。|
|[更新 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|更新 [mobileAppInstallStatus 对象](../resources/intune-apps-mobileappinstallstatus.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceName|String|设备名称|
|deviceId|String|设备 ID|
|lastSyncDateTime|DateTimeOffset|上次同步日期时间|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-apps-resultantappstate.md)|应用的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|installState|[resultantAppState](../resources/intune-apps-resultantappstate.md)|应用的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|应用的安装状态详细信息。 可能的值是 `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` ：、、、、、、、、、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `supersededAppUninstallFailed` `supersededAppUninstallPendingReboot` `removingSupersededApps` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `uninstallPendingReboot` `supersedingAppsDetected` `supersededAppsDetected` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `untargetedSupersedingAppsDetected` `appRemovedBySupersedence` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `supersedingAppsNotApplicable` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable`|
|errorCode|Int32|安装或卸载失败的错误代码。|
|osVersion|String|操作系统版本|
|osDescription|String|操作系统说明|
|userName|String|设备用户名|
|userPrincipalName|String|用户主体名称|
|displayVersion|String|应用程序的可读人工版本|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|应用|[mobileApp](../resources/intune-shared-mobileapp.md)|指向移动应用的导航链接。|

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



