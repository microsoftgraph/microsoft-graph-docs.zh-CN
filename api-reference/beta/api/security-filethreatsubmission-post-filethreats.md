---
title: 创建 fileThreatSubmission
description: 创建新的 fileThreatSubmission 对象。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9d90f57f4d40f461d98913078a294199b1b786be
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856524"
---
# <a name="create-filethreatsubmission"></a>创建 fileThreatSubmission
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [fileThreatSubmission](../resources/security-filethreatsubmission.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ThreatSubmission.ReadWrite，ThreatSubmission.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|ThreatSubmission.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/threatSubmission/fileThreats
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [fileContentThreatSubmission](../resources/security-filecontentthreatsubmission.md) 对象的 JSON 表示形式。 [fileUrlContentThreatSubmission](../resources/security-fileurlthreatsubmission.md) 是保留的，从今天起不受支持。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [fileThreatSubmission](../resources/security-filethreatsubmission.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_filethreatsubmission_from_filethreats"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/threatSubmission/fileThreatSubmissions
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.fileContentThreatSubmission",
  "category": "malware",
  "fileName": "test.html",
  "fileContent": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}
```


### <a name="response"></a>响应
下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.fileThreatSubmission"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/threatSubmission/fileThreatSubmission/$entity",
  "@odata.type": "#microsoft.graph.fileThreatSubmission",
  "category": "malware",
  "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
  "createdDateTime": "2021-10-10T03:30:18.6890937Z",
  "contentType": "file",
  "fileName": "test.html",
  "status": "running",
  "source": "administrator",
  "createdBy": {
    "user": {
      "identity": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin",
      "email": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com"
    }
  },
  "result": {
    "detail": "underInvestigation"
  },
  "adminReview": null,
  "tenantId" : "39238e87-b5ab-4ef6-a559-af54c6b07b42"
}
```

