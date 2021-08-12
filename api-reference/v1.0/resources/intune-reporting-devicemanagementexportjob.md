---
title: deviceManagementExportJob 资源类型
description: 表示要导出报告的作业的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea4c3938edb1de14d605065d20b4bc3a53b1d7abdcfa69ccf3d5bd334a0c4cf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231591"
---
# <a name="devicemanagementexportjob-resource-type"></a>deviceManagementExportJob 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示要导出报告的作业的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementExportJobs](../api/intune-reporting-devicemanagementexportjob-list.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 集合|列出 [deviceManagementExportJob 对象的属性和](../resources/intune-reporting-devicemanagementexportjob.md) 关系。|
|[获取 deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|读取 [deviceManagementExportJob 对象的属性和](../resources/intune-reporting-devicemanagementexportjob.md) 关系。|
|[创建 deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-create.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|创建新的 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象。|
|[删除 deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-delete.md)|无|删除 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)。|
|[更新 deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|更新 [deviceManagementExportJob 对象](../resources/intune-reporting-devicemanagementexportjob.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|
|reportName|String|报告的名称|
|filter|String|应用于报表的筛选器|
|select|String collection|从报表选择的列|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|导出的报告的格式。 可取值为：`csv`、`pdf`。|
|snapshotId|String|快照是由 ReportName 表示的数据集的可识别子集。 可以在此处使用 sessionId 或 CachedReportConfiguration ID。 如果指定了 sessionId，则 Filter、Select 和 OrderBy 将应用于 sessionId 表示的数据。 Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。|
|localizationType|[deviceManagementExportJobLocalizationType](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|配置所请求的导出作业的本地化方式。 可取值为：`localizedValuesAsAdditionalColumn`、`replaceLocalizableValues`。|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|导出作业的状态。 可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。|
|url|String|导出报告的临时位置|
|requestDateTime|DateTimeOffset|请求导出报告的时间|
|expirationDateTime|DateTimeOffset|导出报告的过期时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExportJob"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "format": "String",
  "snapshotId": "String",
  "localizationType": "String",
  "status": "String",
  "url": "String",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```




