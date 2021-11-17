---
title: 获取 bitlockerRecoveryKey
description: 检索 bitlockerRecoveryKey 对象的属性和关系。
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1a7da6ef2b5bf4fbedc75410a228f54460b30d80
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001104"
---
# <a name="get-bitlockerrecoverykey"></a>获取 bitlockerRecoveryKey
命名空间：microsoft.graph

检索 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象的属性和关系。 

默认情况下，此操作不会返回表示实际恢复密钥的 key 属性。 若要在 **响应中包括 key** 属性，请使用 `$select` OData 查询参数。 包含 `$select` 查询参数将触发Azure AD审核操作并生成一个审核日志。 有关 bitlocker 恢复密钥的审核日志详细信息，请参阅适用于 bitlocker 恢复密钥的 KeyManagement [Azure AD筛选器](/azure/active-directory/reports-monitoring/concept-audit-logs)。

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
在不返回 key 属性的情况下获取指定的 BitLocker **密钥：**
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/{bitlockeryRecoveryKeyId}
```

若要获取指定的 BitLocker 密钥（包括其 **key** 属性）：
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/{bitlockeryRecoveryKeyId}?$select=key
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` OData 查询参数返回 **key** 属性。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|ocp-client-name|执行 API 调用的客户端应用程序的名称。 此标头用于调试目的。 可选。|
|ocp-client-version|执行 API 调用的客户端应用程序的版本。 此标头用于调试目的。 可选。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-get-the-bitlocker-key-by-specifying-the-key-id"></a>示例 1：通过指定密钥 ID 获取 BitLocker 密钥

#### <a name="request"></a>请求
下面展示了示例请求。 本示例不返回 **key** 属性。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-bitlockerrecoverykey-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "2020-06-15T13:45:30.0000000Z",
    "volumeType": "1",
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
  }
}
```

### <a name="example-2-get-the-bitlocker-key-with-the-key-property"></a>示例 2：获取具有 **key** 属性的 BitLocker 密钥

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey_key"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-key-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-key-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-key-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-key-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-bitlockerrecoverykey-key-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "String (timestamp)",
    "volumeType": "1",
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
    "key": "123456-231453-873456-213546-654678-765689-123456-324565"
  }
}
```
