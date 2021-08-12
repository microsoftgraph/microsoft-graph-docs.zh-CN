---
title: 更新 deviceManagementExportJob
description: 更新 deviceManagementExportJob 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8a510a2dbe9d80305e04d729f3aae718918194114f80e08cb14bfb26010f089
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249424"
---
# <a name="update-devicemanagementexportjob"></a>更新 deviceManagementExportJob

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceManagementExportJob 对象](../resources/intune-reporting-devicemanagementexportjob.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象的 JSON 表示形式。

下表显示创建 [deviceManagementExportJob 时所需的属性](../resources/intune-reporting-devicemanagementexportjob.md)。

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



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




