---
title: 列出用户
description: 列出 user 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e72ab04776bdf56c7e4896c5f94d8f97481ff446
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702908"
---
# <a name="list-users"></a>列出用户

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件

若要调用此 API，必须有以下权限之一。 要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。  特定权限取决于上下文。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All |
| &nbsp; &nbsp; **载入** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **故障排除** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All |
| &nbsp; &nbsp; **载入** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **故障排除** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a>请求标头

|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```











