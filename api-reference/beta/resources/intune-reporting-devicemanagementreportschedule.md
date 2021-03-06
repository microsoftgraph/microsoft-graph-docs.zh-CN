---
title: deviceManagementReportSchedule 资源类型
description: 表示为其传递报告的计划的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 121940d6bad85ed63589ae62254e667d7fd81c0e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307092"
---
# <a name="devicemanagementreportschedule-resource-type"></a>deviceManagementReportSchedule 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示为其传递报告的计划的实体

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 deviceManagementReportSchedules](../api/intune-reporting-devicemanagementreportschedule-list.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 集合|列出 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的属性和关系。|
|[获取 deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|读取 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的属性和关系。|
|[创建 deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-create.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|创建新的 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象。|
|[删除 deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-delete.md)|无|删除 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)。|
|[更新 deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|更新 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|此实体的唯一标识符|
|reportScheduleName|字符串|计划的名称|
|subject|String|已传递的计划报告的主题|
|电子邮件|String 集合|计划报告传递到的电子邮件|
|recurrence|[deviceManagementScheduledReportRecurrence](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|计划报告传递的频率。 可取值为：`none`、`daily`、`weekly`、`monthly`。|
|startDateTime|DateTimeOffset|计划报告的开始交付时间|
|endDateTime|DateTimeOffset|计划报告的结束传递时间|
|userId|字符串|创建报表的用户的 Id|
|reportName|字符串|报告的名称|
|filter|字符串|在报表上应用的筛选器|
|select|String 集合|从报告中选择的列|
|By|String 集合|报表中的列的排序|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|计划报告的格式。 可取值为：`csv`、`pdf`。|

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




