---
title: 创建 educationClass
description: 创建新的 educationClass 对象。
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 38ab75a0a539088c4e1d1b67380875276dba47dd
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60937347"
---
# <a name="create-educationclass"></a>创建 educationClass

命名空间：microsoft.graph

创建新的 [educationClass](../resources/educationclass.md) 对象。

> [!NOTE]
> 此操作还会创建通用组。 使用此 API 创建课程时，它会向组添加特殊属性，这将在使用组创建团队时在 Microsoft Teams 中添加分配和特殊处理等功能。 请注意，此 API 仅创建通用组，不会创建团队。 Microsoft Teams为教师提供了用户界面，以使用此 API 创建的组创建自己的班级团队。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | 不支持。                              |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/classes
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。

下表显示创建 [educationClass](../resources/educationclass.md)时所需的属性。

| 属性             | 类型                                           | 说明                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| id                   | String                                         | 对象标识符。 继承自 [实体](../resources/entity.md) |
| displayName          | String                                         | 课程名称。                                                 |
| mailNickname         | String                                         | 向所有成员发送电子邮件的邮件名称（如果已启用）。    |
| description          | String                                         | 课程说明。                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | 创建了课程的实体                                       |
| classCode            | String                                         | 学校用于标识课程的课程代码。               |
| externalName         | String                                         | 同步系统中的课程名称。                           |
| externalId           | String                                         | 来自同步系统的课程 ID。                           |
| externalSource       | educationExternalSource                        | 此课程的创建方式。 可能的值包括： `sis` 、 `manual`   |
| externalSourceDetail | String                                         | 生成此资源的外部源的名称。 |
| grade                | String                                         | 课程的年级。                                          |
| term                 | [educationTerm](../resources/educationterm.md) | 此课程的学期。                                               |

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationClass](../resources/educationclass.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
