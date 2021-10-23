---
title: 更新设备
description: 更新已注册设备的属性。
author: sandeo-MSFT
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8392eb7acf846f21e0e60e750ca89c3e2af4962f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558824"
---
# <a name="update-device"></a>更新设备

命名空间：microsoft.graph

更新已注册设备的属性。

设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.ReadWrite.All、Directory.AccessAsUser.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application | Device.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

`{id}`请求中的 是设备的 **id** 属性的值，而不是 **deviceId** 属性的值。
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```


## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的 [device](../resources/device.md) 属性值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了实现最佳性能，不得添加未变化的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 启用帐户时为 `true`，否则为 `false`。 只有全局管理员和云设备管理员角色中的呼叫者才能更新此属性。|
|operatingSystem|String|设备上的操作系统类型。|
|operatingSystemVersion|String|设备上的操作系统版本|
|displayName|String|设备显示名称。|
|isCompliant|Boolean|`true` 如果设备符合移动设备管理 (MDM) 策略;否则为 `false` 。 这仅可通过 Intune 针对任何设备操作系统类型进行更新，或由适用于任何操作系统设备的已批准[MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) Windows更新。 |
|isManaged|Boolean|`true` 如果设备由移动设备管理中心管理， (MDM) 应用;否则为 `false` 。 这仅可通过 Intune 针对任何设备操作系统类型进行更新，或由适用于任何操作系统设备的已批准[MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) Windows更新。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-update-the-accountenabled-property-of-a-device"></a>示例 1：更新设备的 accountEnabled 属性

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json

{
  "accountEnabled": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2--write-extensionattributes-on-a-device"></a>示例 2：在设备上写入 extensionAttributes

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_device_extensionAttributes"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json

{
    "extensionAttributes": {
        "extensionAttribute1": "BYOD-Device"
    }
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
