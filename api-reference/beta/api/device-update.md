---
title: 更新设备
description: 更新设备的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ebdcaf5044ddaefcc1cdbcc385ff0b35d8b8b746
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862636"
---
# <a name="update-device"></a>更新设备

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新设备的属性。

设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.ReadWrite.All、Directory.AccessAsUser.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | 不支持 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> 注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的 [device](../resources/device.md) 属性值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了实现最佳性能，不得添加未变化的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 如果帐户已启用，则为 **true**；否则，为 **false**。 |
|operatingSystem|String|设备上的操作系统类型。|
|operatingSystemVersion|String|设备上的操作系统版本|
|displayName|String|设备显示名称。|
|isCompliant|Boolean|如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。 这只能由 Intune 针对任何设备 OS 类型或经批准的适用于 Windows OS 设备的[MDM 应用](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)进行更新。 |
|isManaged|Boolean|如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。 这只能由 Intune 针对任何设备 OS 类型或经批准的适用于 Windows OS 设备的[MDM 应用](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)进行更新。 |

由于**设备**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用该`PATCH`操作在现有**设备**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

##### <a name="request"></a>请求


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/beta/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据（预览）](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据（预览）](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
