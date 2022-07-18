---
title: managedDevice：bulkRestoreCloudPc
description: 使用单个请求还原多个云电脑设备，其中包括 Intune 托管设备的 ID 和还原点日期和时间。
author: rongting
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 4d86a8502ef40cbf9a53ee1632753c71c6724fa0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338193"
---
# <a name="manageddevice-bulkrestorecloudpc"></a>managedDevice：bulkRestoreCloudPc
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用单个请求还原多个云电脑设备，其中包括 Intune 托管设备的 ID 和还原点日期和时间。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/bulkRestoreCloudPc
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|managedDeviceIds|String 集合|云电脑设备的 ID。|
|restorePointDateTime|DateTimeOffset|所选云电脑设备还原到以前状态 UTC 时间点。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为"2014-01-01T00：00：00Z"。|
|timeRange|[restoreTimeRange](#restoretimerange-values)|还原点的时区。 可能的值是：`before`、`after`、`beforeOrAfter`、`unknownFutureValue`。|

### <a name="restoretimerange-values"></a>restoreTimeRange 值

|成员|说明|
|:---|:---|
|before|选择所选时间点之前最近的快照。|
|after|选择所选时间点后最近的快照。|
|beforeOrAfter|选择与所选时间点最接近的快照。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

## <a name="response"></a>响应

如果成功，此操作在响应 `200 OK` 正文中返回 响应代码和 [cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md) 。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "manageddevicethis.bulkrestorecloudpc"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/bulkRestoreCloudPc
Content-Type: application/json
Content-length: 123

{
  "managedDeviceIds": [
    "30d0e128-de93-41dc-89ec-33d84bb662a0",
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
  ],
  "restorePointDateTime": "2021-09-23T04:00:00.0000000",
  "timeRange": "before"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/manageddevicethisbulkrestorecloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/manageddevicethisbulkrestorecloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/manageddevicethisbulkrestorecloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/manageddevicethisbulkrestorecloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/manageddevicethisbulkrestorecloudpc-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/manageddevicethisbulkrestorecloudpc-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面展示了示例响应。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult",
    "successfulDeviceIds": [
        "30d0e128-de93-41dc-89ec-33d84bb662a0"
    ],
    "failedDeviceIds": [
        "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
    ],
    "notFoundDeviceIds": [
    ],
    "notSupportedDeviceIds": [
    ]
  }
}
```
