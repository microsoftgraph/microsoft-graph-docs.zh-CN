---
title: deviceManagementReports 资源类型
description: 充当所有报表功能容器的单一实例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f05d668ad7397236868f023f76191e46a77e522
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730971"
---
# <a name="devicemanagementreports-resource-type"></a>deviceManagementReports 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有报表功能容器的单一实例实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagementReports](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|读取 [deviceManagementReports 对象的](../resources/intune-reporting-devicemanagementreports.md) 属性和关系。|
|[更新 deviceManagementReports](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|更新 [deviceManagementReports 对象的](../resources/intune-reporting-devicemanagementreports.md) 属性。|
|[getDeviceNonComplianceReport 操作](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Stream|尚未记录|
|[getNoncompliantDevicesAndSettingsReport 操作](../api/intune-reporting-devicemanagementreports-getnoncompliantdevicesandsettingsreport.md)|Stream|尚未记录|
|[getPolicyNonComplianceReport 操作](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|Stream|尚未记录|
|[getPolicyNonComplianceMetadata 操作](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|Stream|尚未记录|
|[getPolicyNonComplianceSummaryReport 操作](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport.md)|Stream|尚未记录|
|[getSettingNonComplianceReport 操作](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|Stream|尚未记录|
|[getReportFilters 操作](../api/intune-reporting-devicemanagementreports-getreportfilters.md)|Stream|尚未记录|
|[getHistoricalReport 操作](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|Stream|尚未记录|
|[getConfigurationPolicyNonComplianceSummaryReport 操作](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancesummaryreport.md)|Stream|尚未记录|
|[getConfigurationPolicyNonComplianceReport 操作](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancereport.md)|Stream|尚未记录|
|[getConfigurationSettingNonComplianceReport 操作](../api/intune-reporting-devicemanagementreports-getconfigurationsettingnoncompliancereport.md)|Stream|尚未记录|
|[getDeviceManagementIntentSettingsReport 操作](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentsettingsreport.md)|Stream|尚未记录|
|[getDeviceManagementIntentPerSettingContributingProfiles 操作](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentpersettingcontributingprofiles.md)|Stream|尚未记录|
|[getCompliancePolicyNonComplianceSummaryReport 操作](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancesummaryreport.md)|Stream|尚未记录|
|[getCompliancePolicyNonComplianceReport 操作](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancereport.md)|Stream|尚未记录|
|[getComplianceSettingNonComplianceReport 操作](../api/intune-reporting-devicemanagementreports-getcompliancesettingnoncompliancereport.md)|Stream|尚未记录|
|[getCachedReport 操作](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|Stream|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|exportJobs|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 集合|表示要导出报表的作业的实体|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```





