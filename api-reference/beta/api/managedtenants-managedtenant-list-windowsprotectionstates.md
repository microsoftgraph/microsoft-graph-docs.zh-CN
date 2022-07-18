---
title: 列出 windowsProtectionStates
description: 获取 windowsProtectionState 对象及其属性的列表。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e7508237b472750c6ca176194bb79543dc1c1fa3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791222"
---
# <a name="list-windowsprotectionstates"></a>列出 windowsProtectionStates
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/windowsProtectionStates
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/windowsProtectionStates
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-windowsprotectionstate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-windowsprotectionstate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-windowsprotectionstate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-windowsprotectionstate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-windowsprotectionstate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.windowsProtectionState)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/windowsProtectionStates",
    "value": [
        {
            "id": "34298981-4fc8-4974-9486-c8909ed1521b_95378ac4-eded-4671-8fa2-4e42e5de3463",
            "managedDeviceId": "95378ac4-eded-4671-8fa2-4e42e5de3463",
            "managedDeviceName": "vm11",
            "malwareProtectionEnabled": true,
            "managedDeviceHealthState": "Clean",
            "realTimeProtectionEnabled": true,
            "networkInspectionSystemEnabled": true,
            "quickScanOverdue": false,
            "fullScanOverdue": false,
            "signatureUpdateOverdue": false,
            "rebootRequired": false,
            "attentionRequired": false,
            "fullScanRequired": false,
            "engineVersion": "1.1.18300.4",
            "signatureVersion": "1.343.642.0",
            "antiMalwareVersion": "4.18.2106.6",
            "lastQuickScanDateTime": "2021-06-24T14:50:28Z",
            "lastFullScanDateTime": null,
            "lastQuickScanSignatureVersion": "1.341.1288.0",
            "lastFullScanSignatureVersion": "0.0.0.0",
            "lastReportedDateTime": "2021-07-09T14:43:45Z",
            "devicePropertiesRefreshTime": "2021-07-09T14:44:28Z",
            "deviceDeleted": false,
            "lastRefreshedDateTime": "2021-07-11T02:02:35.9816065Z",
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
            "tenantDisplayName": "Fourth Coffee",
            "devicePropertiesRefreshDateTime": "2021-07-09T14:44:28Z"
        },
        {
            "id": "38227791-a88b-4fcc-81c5-58cf77668320_49ed91f1-32ac-4881-9c1b-b709ba29e31b",
            "managedDeviceId": "49ed91f1-32ac-4881-9c1b-b709ba29e31b",
            "managedDeviceName": "VM4511",
            "malwareProtectionEnabled": true,
            "managedDeviceHealthState": "Clean",
            "realTimeProtectionEnabled": true,
            "networkInspectionSystemEnabled": true,
            "quickScanOverdue": false,
            "fullScanOverdue": false,
            "signatureUpdateOverdue": false,
            "rebootRequired": false,
            "attentionRequired": false,
            "fullScanRequired": false,
            "engineVersion": "1.1.18300.4",
            "signatureVersion": "1.343.618.0",
            "antiMalwareVersion": "4.18.2105.5",
            "lastQuickScanDateTime": "2021-06-21T15:05:41Z",
            "lastFullScanDateTime": "2021-04-19T20:03:26Z",
            "lastQuickScanSignatureVersion": "1.341.1157.0",
            "lastFullScanSignatureVersion": "1.303.25.0",
            "lastReportedDateTime": "2021-07-09T14:43:52Z",
            "devicePropertiesRefreshTime": "2021-07-09T14:44:28Z",
            "deviceDeleted": false,
            "lastRefreshedDateTime": "2021-07-11T02:02:35.9816065Z",
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
            "tenantDisplayName": "Consolidated Messenger",
            "devicePropertiesRefreshDateTime": "2021-07-09T14:44:28Z"
        }
    ]
}
```
