---
title: wipeManagedAppRegistrationByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 09bb38400433344bc1706be33ff12f5bc663c000
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787053"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a>wipeManagedAppRegistrationByDeviceTag 操作

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本的 API 可能会更改。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对包含指定设备标记的应用注册发布擦除操作。

## <a name="prerequisites"></a>先决条件

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a>请求标头

|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文

在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|属性|类型|说明|
|:---|:---|:---|
|deviceTag|String|设备标记|

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

``` http
HTTP/1.1 204 No Content
```












