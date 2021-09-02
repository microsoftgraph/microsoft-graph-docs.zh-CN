---
title: deviceManagementReportSchedule 资源类型
description: 表示送达报告的计划的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ed97e1cebfec55a6ec9420ab818f208873daa2a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800343"
---
# <a name="devicemanagementreportschedule-resource-type"></a>deviceManagementReportSchedule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示送达报告的计划的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementReportSchedules](../api/intune-reporting-devicemanagementreportschedule-list.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 集合|列出 [deviceManagementReportSchedule 对象的属性和](../resources/intune-reporting-devicemanagementreportschedule.md) 关系。|
|[获取 deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|读取 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的属性和关系。|
|[创建 deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-create.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|创建新的 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。|
|[删除 deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-delete.md)|无|删除 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)。|
|[更新 deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|更新 [deviceManagementReportSchedule 对象](../resources/intune-reporting-devicemanagementreportschedule.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|
|reportScheduleName|String|计划的名称|
|subject|String|已送达的计划报告的主题|
|电子邮件|字符串集合|将计划报告传递到的电子邮件|
|recurrence|[deviceManagementScheduledReportRecurrence](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|计划报告传递的频率。 可取值为：`none`、`daily`、`weekly`、`monthly`。|
|startDateTime|DateTimeOffset|计划报告交付开始的时间|
|endDateTime|DateTimeOffset|计划报告传递结束的时间|
|userId|String|创建报告的用户的 ID|
|reportName|字符串|报告的名称|
|filter|字符串|应用于报表的筛选器|
|select|字符串集合|从报表选择的列|
|orderBy|字符串集合|报告中列的排序|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|计划报表的格式。 可取值为：`csv`、`pdf`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReportSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "String (identifier)",
  "reportScheduleName": "String",
  "subject": "String",
  "emails": [
    "String"
  ],
  "recurrence": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "userId": "String",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "format": "String"
}
```



