---
title: deviceManagementReports 资源类型
description: 充当所有报告功能的容器的单一实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc587c5d7dfacb13b1aec0cba033e5816f49a1cd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751809"
---
# <a name="devicemanagementreports-resource-type"></a>deviceManagementReports 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有报告功能的容器的单一实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagementReports](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|读取 [deviceManagementReports 对象的属性和](../resources/intune-reporting-devicemanagementreports.md) 关系。|
|[更新 deviceManagementReports](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|更新 [deviceManagementReports 对象](../resources/intune-reporting-devicemanagementreports.md) 的属性。|
|[getDeviceNonComplianceReport 操作](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Stream|尚未记录|
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
|exportJobs|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 集合|表示要导出报告的作业的实体|

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




