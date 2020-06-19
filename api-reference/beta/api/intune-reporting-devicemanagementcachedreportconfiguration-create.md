---
title: 创建 deviceManagementCachedReportConfiguration
description: 创建新的 deviceManagementCachedReportConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7340fffa01f99c33433c60b08b12748a2505cfae
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791361"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a>创建 deviceManagementCachedReportConfiguration

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象。

## <a name="prerequisites"></a>先决条件
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceManagementCachedReportConfiguration 对象的 JSON 表示形式。

下表显示创建 deviceManagementCachedReportConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|
|reportName|String|报告的名称|
|filter|String|在创建报表时应用的筛选器。|
|select|String collection|从报告中选择的列|
|By|String collection|报表中的列的排序|
|metadata|String|与报告关联的调用方托管元数据|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|缓存报告的状态。 可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。|
|lastRefreshDateTime|DateTimeOffset|上次刷新缓存的报告的时间|
|expirationDateTime|DateTimeOffset|缓存的报表到期的时间|



## <a name="response"></a>响应
如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
Content-type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a>响应
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 467

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "46947722-7722-4694-2277-944622779446",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```



