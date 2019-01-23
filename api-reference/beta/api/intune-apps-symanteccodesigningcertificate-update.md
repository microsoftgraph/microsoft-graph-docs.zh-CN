---
title: 更新 symantecCodeSigningCertificate
description: 更新 symantecCodeSigningCertificate 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5da263a8b4c2bbf121fb994b4d20168c45da9e03
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414023"
---
# <a name="update-symanteccodesigningcertificate"></a>更新 symantecCodeSigningCertificate

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的 JSON 表示形式。

下表显示时创建[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|content|Binary|中的原始数据格式的 Windows Symantec 代码签名证书。|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|设置或未设置证书的状态。 可取值为：`notProvisioned`、`provisioned`。|
|password|String|.Pfx 文件所需的密码。|
|SubjectName|String|证书使用者名称。|
|subject|String|证书使用者值。|
|issuerName|String|证书颁发者名称。|
|颁发者|String|证书颁发者值。|
|expirationDateTime|DateTimeOffset|证书到期日期。|
|uploadDateTime|DateTimeOffset|作为 Symantec Cert 代码签名证书的类型。|



## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```




