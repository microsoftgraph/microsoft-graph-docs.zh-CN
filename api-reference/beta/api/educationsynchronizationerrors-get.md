---
title: 获取 educationSynchronizationErrors
description: '获取验证期间和/或同步租户中的特定学校数据同步配置文件期间生成的错误。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d652938060bd577a00f1f22c3ce8cb5d5cc8160d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043162"
---
# <a name="get-educationsynchronizationerrors"></a>获取 educationSynchronizationErrors

命名空间：microsoft.graph

获取验证期间和/或同步租户中的特定学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 期间生成的错误。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                       | 权限（从最低特权到最高特权）                 |
| :------------------------------------ | :---------------------------------------------------------- |
| 委派（工作或学校帐户）    | EduAdministration.Read、EduAdministration.ReadWrite         |
| 委派 (个人 Microsoft 帐户 | 不支持。                                              |
| 应用程序                           | EduAdministration.Read.All、EduAdministration.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /education/synchronizationProfiles/{id}/errors
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 [OData](/graph/query-parameters) 查询参数来帮助自定义响应：$filter、$orderby、$top、$skip 和 \$ count。

## <a name="request-headers"></a>请求标头

| 名称          | 类型   | 说明               |
| :------------ | :----- | :------------------------ |
| Authorization | string | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [同步错误](../resources/educationsynchronizationerror.md) 对象集合。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-error-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/errors",
  "@odata.count": 14,
  "value": [
    {
      "id": "92797B7C-02C3-4326-8ACC-E81C78753831",
      "entryType": "Student",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
      "joiningValue": "richard.2wilson@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:45Z",
      "reportableIdentifier": "richard.2wilson"
    },
    {
      "id": "94C1EB0E-8339-4EF4-8CB2-EB15C6228CE1",
      "entryType": "Teacher",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
      "joiningValue": "alberto2.dorsey@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:57Z",
      "reportableIdentifier": "alberto2.dorsey"
    },
    {
      "id": "98A82052-7716-49E9-90CC-C6FF406FC8E5",
      "entryType": "Teacher",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
      "joiningValue": "madeline2.bullock@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:57Z",
      "reportableIdentifier": "madeline2.bullock"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
