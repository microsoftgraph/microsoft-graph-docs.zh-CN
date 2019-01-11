---
title: 删除用户
description: 删除 user。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc1979284cada76f76a98acc8956271b7224aa53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837833"
---
# <a name="delete-user"></a>删除 user

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

删除 [user](../resources/intune-shared-user.md)。
## <a name="prerequisites"></a>先决条件
以下权限之一需要调用此 API。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。  所需的特定权限取决于上下文。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）| _随上下文_|
| &nbsp;&nbsp;设备 | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; MAM | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp;入职培训 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;疑难解答 | DeviceManagementManagedDevices.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

``` http
HTTP/1.1 204 No Content
```



