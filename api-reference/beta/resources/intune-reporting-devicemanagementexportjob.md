---
title: deviceManagementExportJob 资源类型
description: 表示要导出报表的作业的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bef520a455a702e2f9f8c2a0926581b01e8d7418
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440190"
---
# <a name="devicemanagementexportjob-resource-type"></a>deviceManagementExportJob 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示要导出报表的作业的实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementExportJobs](../api/intune-reporting-devicemanagementexportjob-list.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 集合|列出 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象的属性和关系。|
|[获取 deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|读取 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象的属性和关系。|
|[创建 deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-create.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|创建新的 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象。|
|[删除 deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-delete.md)|无|删除 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)。|
|[更新 deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|更新 [deviceManagementExportJob 对象](../resources/intune-reporting-devicemanagementexportjob.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|
|reportName|String|报告的名称|
|filter|String|应用于报表的筛选器|
|select|字符串集合|从报告中选择的列|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|导出报表的格式。 可取值为：`csv`、`pdf`。|
|snapshotId|String|快照是由 ReportName 表示的数据集的可识别子集。 可以在此处使用 sessionId 或 CachedReportConfiguration ID。 如果指定了 sessionId，则 Filter、Select 和 OrderBy 将应用于 sessionId 表示的数据。 不能将 Filter、Select 和 OrderBy 与 CachedReportConfiguration ID 一起指定。|
|localizationType|[deviceManagementExportJobLocalizationType](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|配置如何本地化请求的导出作业。 可取值为：`localizedValuesAsAdditionalColumn`、`replaceLocalizableValues`。|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|导出作业的状态。 可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。|
|url|String|导出的报告的临时位置|
|requestDateTime|DateTimeOffset|请求导出报告的时间|
|expirationDateTime|DateTimeOffset|导出报告过期的时间|

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




