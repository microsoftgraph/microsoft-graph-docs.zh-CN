---
title: deviceManagementCachedReportConfiguration 资源类型
description: 表示缓存报告配置的实体
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34db21fc0e010a118077e90ad543e40b06da6884
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772669"
---
# <a name="devicemanagementcachedreportconfiguration-resource-type"></a>deviceManagementCachedReportConfiguration 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示缓存报告配置的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementCachedReportConfigurations](../api/intune-reporting-devicemanagementcachedreportconfiguration-list.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)集合|列出[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性和关系。|
|[获取 deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-get.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|读取[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性和关系。|
|[创建 deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-create.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|创建新的[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象。|
|[删除 deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-delete.md)|None|删除[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)。|
|[更新 deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-update.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|更新[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|
|reportName|String|报告的名称|
|filter|String|在创建报表时应用的筛选器。|
|select|String collection|从报告中选择的列|
|By|String collection|报表中的列的排序|
|状态|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|缓存报告的状态。 可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。|
|lastRefreshDateTime|DateTimeOffset|上次刷新缓存的报告的时间|
|expirationDateTime|DateTimeOffset|缓存的报表到期的时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCachedReportConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "status": "String",
  "lastRefreshDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



