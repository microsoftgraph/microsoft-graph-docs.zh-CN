---
title: 列出 teamworkDevices
description: 获取为租户预配Microsoft Teams已启用设备的列表。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 2598b334e858a2e58507d95894ad48d596a9e1d9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342565"
---
# <a name="list-teamworkdevices"></a>列出 teamworkDevices
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取为租户Microsoft Teams已启用设备的列表。[](../resources/teamworkdevice.md)

[!INCLUDE [teamworkdevice-api-disclaimer](../../includes/teamworkdevice-api-disclaimer.md)]

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|TeamworkDevice.Read.All、TeamworkDevice.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|TeamworkDevice.Read.All、TeamworkDevice.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/devices
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$filter` (**deviceType**、**hardwareDetail/uniqueId** 和 **currentUser/id** 属性) 、、 `$top``$select``$skipToken` 和 [OData](/graph/query-parameters) 查询参数来帮助自定义响应。

### <a name="supported-query-patterns"></a>支持的查询模式

| 模式                | 语法                                 | 备注 |
| ---------------------- | -------------------------------------- | ----- |
| 服务器端分页 | `@odata.nextLink`                      | 当一个事件跨多个页面时，你将在响应结果集延续令牌。 |
| 筛选器                 | `/devices?$filter=deviceType eq 'TeamsRoom'` | 根据设备类别筛选设备。 |
| 筛选器                 | `/devices?$filter=hardwareDetail/uniqueId eq 'value'` | 基于分配给设备的 **uniqueId** 筛选设备。 |
| 筛选器                 | `/devices?$filter=currentUser/id eq 'value'` |  基于设备上已登录的用户筛选设备。|
| 页面限制             | `/devices?$top=10` | 获取页面大小为 10 的设备。 默认页面限制为 20。 最大页面限制为 50。 |

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码 [和 teamworkDevice](../resources/teamworkdevice.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamworkdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamworkdevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamworkdevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamworkdevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamworkdevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamworkdevice-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-teamworkdevice-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDevice",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teamwork/devices",
  "@odata.count": 2,
  "@odata.nextLink": "/teamwork/devices?$filter=deviceType+eq+Microsoft.Teams.GraphSvc.teamworkDeviceType%collaborationBar%27&$top=2&$skiptoken=%2bRID%3a~z9snAP1BE88Zlz0AAAAADg%3d%3d%23RT%3a1%23TRC%3a3%23RTD%3auCNd2ZP%2fZ5zLgoPeFGRGBTMxMzIuMTcuMzJVMTY7NTc7MjEvNTozNjEyM1sA%23ISV%3a2%23IEO%3a65551%23QCF%3a4%23FPC%3aAggBAAAAADgAAPcAAAAAOAAAAQAAAAA4AAACADiI9AAAAAA4AAACABCP9QAAAAA4AAAEAFEu4AD2AAAAADgAAAQANoXZkfcAAAAAOAAABAAlgIiK",
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamworkDevice",
      "id": "0f3ce432-e432-0f3c-32e4-3c0f32e43c0f",
      "deviceType": "CollaborationBar",
      "hardwareDetail": {
        "serialNumber": "0189",
        "uniqueId": "5abcdefgh",
        "macAddresses": [],
        "manufacturer": "yealink",
        "model": "vc210"
      },
      "notes": "CollaborationBar device.",
      "companyAssetTag": "Tag1",
      "healthStatus": "Healthy",
      "activityState": "Idle",
      "createdDateTime": "2021-06-19T19:01:04.185Z",
      "createdBy": null,
      "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
      "lastModifiedBy": null,
      "currentUser": {
        "id": "2a610f6f-adf6-4205",
        "displayName": "Evan Lewis",
        "userIdentityType": "aadUser"
      }
    },
    {
      "@odata.type": "#microsoft.graph.teamworkDevice",
      "id": "55ab555-e432-0f3c-32e4-3c0f32e43c0f",
      "deviceType": "CollaborationBar",
      "hardwareDetail": {
        "serialNumber": "0189",
        "uniqueId": "5abcdefgh",
        "macAddresses": [],
        "manufacturer": "yealink",
        "model": "vc210"
      },
      "notes": "CollaborationBar device.",
      "companyAssetTag": "Tag2",
      "healthStatus": "Healthy",
      "activityState": "Idle",
      "createdDateTime": "2021-06-10T19:01:04.185Z",
      "createdBy": null,
      "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
      "lastModifiedBy": null,
      "currentUser": {
        "id": "2a610f6f-adf6-4205",
        "displayName": "Evan Lewis",
        "userIdentityType": "aadUser"
      }
    }
  ]
}
```

