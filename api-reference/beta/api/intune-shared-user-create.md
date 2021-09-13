---
title: 创建用户
description: 新建用户对象。
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26ee57b3892d72706900bd633c29b2ef7b32912c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064663"
---
# <a name="create-user"></a>创建用户

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本的 API 可能会更改。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [user](../resources/intune-shared-user.md) 对象。

## <a name="prerequisites"></a>先决条件

若要调用此 API，需要以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。  所需的特定权限取决于上下文。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|
| &nbsp; &nbsp; **载入** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **疑难解答** | DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|
| &nbsp; &nbsp; **载入** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **疑难解答** | DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a>请求标头

|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文

在请求正文中，提供 user 对象的 JSON 表示形式。

下表显示创建 user 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户的唯一标识符。|
|**上机**||
|deviceEnrollmentLimit|Int32|允许用户注册的最大设备数的限制。 允许的值为 5 或 1000。|

请求正文属性支持因上下文而异。

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a>响应

下面是一个响应示例。 注意：为简洁起见，可能会截断此处显示的响应对象。 从实际调用返回的属性因上下文而异。

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









