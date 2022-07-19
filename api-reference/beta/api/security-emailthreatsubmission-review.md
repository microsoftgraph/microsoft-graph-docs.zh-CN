---
title: emailThreatSubmission：查看
description: 查看威胁提交。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9514f417b77c02b88ff6668165cd72daeeb36d4c
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856534"
---
# <a name="emailthreatsubmission-review"></a>emailThreatSubmission：查看
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

查看威胁提交。 只有最终用户提交的 [emailThreatSubmission](../resources/security-emailthreatsubmission.md) 对象才支持审阅操作。

最终用户不支持 [查看 urlThreatSubmission](../resources/security-urlthreatsubmission.md) 和 [fileThreatSubmission](../resources/security-filethreatsubmission.md) 对象的操作。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ThreatSubmission.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|ThreatSubmission.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /emailThreats/{emailThreatsId}/review
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|Description|
|:---|:---|:---|
|“类别”|String|电子邮件被报告为 notSpam、垃圾、网络钓鱼、恶意软件。 不区分大小写。|



## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "emailthreatsubmissionthis.review"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/threatSubmission/emailThreats/49c5ef5b-1f65-444a-e6b9-08d772ea2059/review
Content-type: application/json

{
  "category": "phishing"
}
```


### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

