---
title: deviceManagementCachedReportConfiguration 资源类型
description: 表示缓存报表的配置的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff8d125f6703b1984eb9369bcfa3cd9b75b12249
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793787"
---
# <a name="devicemanagementcachedreportconfiguration-resource-type"></a>deviceManagementCachedReportConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示缓存报表的配置的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementCachedReportConfigurations](../api/intune-reporting-devicemanagementcachedreportconfiguration-list.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 集合|列出 [deviceManagementCachedReportConfiguration 对象的属性和](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 关系。|
|[获取 deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-get.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|读取 [deviceManagementCachedReportConfiguration 对象的属性和](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 关系。|
|[创建 deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-create.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|创建新的 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 对象。|
|[删除 deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-delete.md)|无|删除 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)。|
|[更新 deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-update.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|更新 [deviceManagementCachedReportConfiguration 对象](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|
|reportName|String|报告的名称|
|filter|String|创建报表时应用的筛选器。|
|select|字符串集合|从报表选择的列|
|orderBy|字符串集合|报告中列的排序|
|metadata|String|与报告关联的呼叫者管理的元数据|
|状态|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|缓存报表的状态。 可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。|
|lastRefreshDateTime|DateTimeOffset|上次刷新缓存报告的时间|
|expirationDateTime|DateTimeOffset|缓存报告的过期时间|

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
  "metadata": "String",
  "status": "String",
  "lastRefreshDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



