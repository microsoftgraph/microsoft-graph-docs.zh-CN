---
title: mobileAppInstallStatus 资源类型
description: 包含设备移动应用安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efcf9d78aecd7ba49e5630473e790d3ed7c37406
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671231"
---
# <a name="mobileappinstallstatus-resource-type"></a>mobileAppInstallStatus 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备移动应用安装状态的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合|列出 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。|
|[获取 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|读取 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。|
|[创建 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|创建新的 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象。|
|[删除 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-delete.md)|None|删除 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。|
|[更新 mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|更新 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceName|String|设备名称|
|deviceId|String|设备 ID|
|lastSyncDateTime|DateTimeOffset|上次同步日期时间|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-apps-resultantappstate.md)|应用的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|installState|[resultantAppState](../resources/intune-apps-resultantappstate.md)|应用的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|应用的安装状态详细信息。 可能的值为：、、、、`dependencyWithAutoInstallDisabled``dependencyPendingReboot`、`supersededAppUninstallFailed`、`supersededAppUninstallPendingReboot`、`removingSupersededApps`、`iosAppStoreUpdateFailedToInstall`、`vppAppHasUpdateAvailable`、`userRejectedUpdate`、`supersedingAppsDetected``uninstallPendingReboot``supersededAppsDetected`、`seeInstallErrorCode`、`managedAppNoLongerPresent``autoInstallDisabled`、、、、 `userIsNotLoggedIntoAppStore``installingDependencies``contentDownloaded``pendingReboot``seeUninstallErrorCode``appRemovedBySupersedence``untargetedSupersedingAppsDetected``minimumDiskSpaceNotMet``fileSystemRequirementNotMet``platformNotApplicable``minimumCpuSpeedNotMet``registryRequirementNotMet``minimumPhysicalMemoryNotMet``processorArchitectureNotApplicable``minimumLogicalProcessorCountNotMet``supersedingAppsNotApplicable``powerShellScriptRequirementNotMet``minimumOsVersionNotMet``userRejectedInstall``dependencyWithRequirementsNotMet``dependencyFailedToInstall``noAdditionalDetails`|
|errorCode|Int32|安装或卸载故障的错误代码。|
|osVersion|String|操作系统版本|
|osDescription|String|OS 说明|
|userName|String|设备用户名|
|userPrincipalName|String|用户主体名称|
|displayVersion|String|应用程序的人工可读版本|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|应用|[mobileApp](../resources/intune-apps-mobileapp.md)|移动应用的导航链接。|

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




