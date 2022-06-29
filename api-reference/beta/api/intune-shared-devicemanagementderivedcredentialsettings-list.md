---
title: 列出 deviceManagementDerivedCredentialSettingses
description: 列出 deviceManagementDerivedCredentialSettings 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72783a8b31b73803d9fc9faa04c948de2e1260dc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445284"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a>列出 deviceManagementDerivedCredentialSettingses

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [deviceManagementDerivedCredentialSettings 对象的](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 属性和关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
|&nbsp;&nbsp; **资源访问策略**|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
|&nbsp;&nbsp; **资源访问策略**|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
      "id": "bc650741-0741-bc65-4107-65bc410765bc",
      "helpUrl": "https://example.com/helpUrl/",
      "displayName": "Display Name value",
      "issuer": "entrustDatacard",
      "notificationType": "companyPortal"
    }
  ]
}
```







