---
title: 列出 managedAppStatusRaws
description: 列出 managedAppStatusRaw 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b06804e8c91e668703b67803a13a901bba0f8d0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212515"
---
# <a name="list-managedappstatusraws"></a>列出 managedAppStatusRaws

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatusRaw",
      "displayName": "Display Name value",
      "id": "80847581-7581-8084-8175-848081758480",
      "version": "Version value",
      "content": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```




