---
title: 更新 symantecCodeSigningCertificate
description: 更新 symantecCodeSigningCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 31cecc26dcb6e90fa4e9b5958dfada5e7b31ad8f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802934"
---
# <a name="update-symanteccodesigningcertificate"></a>更新 symantecCodeSigningCertificate

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [symantecCodeSigningCertificate 对象](../resources/intune-apps-symanteccodesigningcertificate.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementApps.ReadWrite.All|

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
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) 对象的 JSON 表示形式。

下表显示创建 [symantecCodeSigningCertificate 时所需的属性](../resources/intune-apps-symanteccodesigningcertificate.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|content|二进制|The Windows Symantec Code-Signing Certificate in the raw data format.|
|状态|[certificateStatus](../resources/intune-apps-certificatestatus.md)|已设置或未预配证书状态。 可取值为：`notProvisioned`、`provisioned`。|
|密码|String|.pfx 文件所需的密码。|
|SubjectName|String|证书的主题名称。|
|subject|String|证书的 Subject 值。|
|issuerName|字符串|证书的颁发者名称。|
|issuer|字符串|证书的 Issuer 值。|
|expirationDateTime|DateTimeOffset|证书到期日期。|
|uploadDateTime|DateTimeOffset|作为 Symantec 证书的 CodeSigning 证书的类型。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) 对象。

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



