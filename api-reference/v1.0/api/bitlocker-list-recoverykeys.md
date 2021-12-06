---
title: 列出 recoveryKeys
description: 获取 bitlockerRecoveryKey 对象及其属性的列表。
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ef1b2ea53996d7a1d97049f275cafb2f18b5fafb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001146"
---
# <a name="list-recoverykeys"></a>列出 recoveryKeys

命名空间：microsoft.graph

获取 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象及其属性的列表。 

此操作不会返回 **key** 属性。 若要了解如何读取 key 属性 **，请参阅** 获取 [bitlockerRecoveryKey](bitlockerrecoverykey-get.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|BitLockerKey.ReadBasic.All、BitLockerKey.Read.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|不支持|

对于委派权限，调用用户必须是最初备份 BitLocker 恢复密钥的设备注册所有者，或者他们必须具有以下目录角色 [之一](/azure/active-directory/roles/permissions-reference)：

* 全局管理员
* 云设备管理员
* 支持人员管理员
* Intune 服务管理员
* 安全管理员
* 安全读者
* 全局读取者

## <a name="http-request"></a>HTTP 请求

若要获取租户内的 BitLocker 密钥列表，请进行以下操作：

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /informationProtection/bitlocker/recoveryKeys
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 查询参数，以按最近备份密钥的设备的 `$filter` **deviceId** 筛选结果。 此方法不支持 `$top` 。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

该响应可能还包含 `odata.nextLink` ，您可以使用 它分页浏览结果集。 有关详细信息，请参阅分页[Microsoft Graph数据](/graph/paging)。

## <a name="request-headers"></a>请求头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|ocp-client-name|执行 API 调用的客户端应用程序的名称。 此标头用于调试目的。 可选。|
|ocp-client-version|执行 API 调用的客户端应用程序的版本。 此标头用于调试目的。 可选。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-retrieve-a-list-of-bitlocker-keys-in-the-tenant"></a>示例 1：检索租户中的 BitLocker 密钥列表。

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-bitlockerrecoverykey-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": "1",
      "deviceId": "2ef04ef1-23b0-2e00-a3a5-ab345e567ab6"
    },
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "6a30ed7b-247b-4d26-86b5-2f405e55ea42",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": "1",
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```

### <a name="example-2-retrieve-a-list-of-bitlocker-keys-filtered-by-deviceid"></a>示例 2：检索按 deviceId 筛选的 BitLocker 密钥列表。

#### <a name="request"></a>请求

下面展示了示例请求。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_bitlockerrecoverykey_filter_deviceId"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-bitlockerrecoverykey-filter-deviceid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-bitlockerrecoverykey-filter-deviceid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-bitlockerrecoverykey-filter-deviceid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-bitlockerrecoverykey-filter-deviceid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-bitlockerrecoverykey-filter-deviceid-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": "1",
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
