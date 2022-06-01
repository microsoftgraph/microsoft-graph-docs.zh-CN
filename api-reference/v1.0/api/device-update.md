---
title: 更新设备
description: 更新已注册设备的属性。
author: sandeo-MSFT
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 183155c31a69c0f669d4bafcaa19cb0a6fa78ee4
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821132"
---
# <a name="update-device"></a>更新设备

命名空间：microsoft.graph

更新已注册设备的属性。

设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。

> [!IMPORTANT]
> 此 API 存在一个[已知问题](/graph/known-issues#linux-based-devices-cant-be-updated-by-an-app-with-application-permissions)。 具有应用程序权限的应用只能更新基于 Linux 的设备的 **extensionAttributes** 属性，即 **operationSystem** 属性所在的 `linux`位置。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Device.ReadWrite.All、Directory.ReadWrite.All |

调用用户还必须具有以下 [Azure AD 角色](/azure/active-directory/roles/permissions-reference)之一：*全局管理员**、Intune管理员*。 *云设备管理员* 角色中的调用用户只能使用此 API 启用或禁用设备，具有 *Windows 365管理员角色的* 用户只能更新基本设备属性。

## <a name="http-request"></a>HTTP 请求

请求 `{id}` 中是设备 **ID 属性的** 值，而不是 **deviceId** 属性的值。
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
|accountEnabled|Boolean| 启用帐户时为 `true`，否则为 `false`。 只有 *全局管理员* 和 *云设备管理员* 角色中的调用方才能更新此属性。|
|operatingSystem|String|设备上的操作系统类型。|
|operatingSystemVersion|String|设备上的操作系统版本|
|displayName|String|设备显示名称。|
|isCompliant|Boolean|`true`如果设备符合移动设备管理 (MDM) 策略，则为 ɭ;否则为 `false`。 这只能通过任何设备 OS 类型的Intune或Windows OS 设备的[已批准 MDM 应用](/windows/client-management/mdm/azure-active-directory-integration-with-mdm)进行更新。 |
|isManaged|Boolean|`true`如果设备由移动设备管理 (MDM) 应用管理，则为 ！;否则为 `false`。 这只能通过任何设备 OS 类型的Intune或Windows OS 设备的[已批准 MDM 应用](/windows/client-management/mdm/azure-active-directory-integration-with-mdm)进行更新。 |

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
PATCH https://graph.microsoft.com/v1.0/devices/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac
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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-device-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-device-powershell-snippets.md)]
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



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device_extensionAttributes"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/devices/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac
Content-type: application/json

{
    "extensionAttributes": {
        "extensionAttribute1": "BYOD-Device"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-extensionattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-extensionattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-device-extensionattributes-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-device-extensionattributes-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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
