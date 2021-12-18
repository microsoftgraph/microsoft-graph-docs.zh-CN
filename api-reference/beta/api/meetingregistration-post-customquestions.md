---
title: 创建 meetingRegistrationQuestion
description: 创建与 meetingRegistration 对象关联的自定义会议注册问题。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0dbbf42b3beaeb46538e2ea230a5e3a34892bb87
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2021
ms.locfileid: "61561501"
---
# <a name="create-meetingregistrationquestion"></a>创建 meetingRegistrationQuestion

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 [组织者创建与](../resources/meetingregistrationquestion.md) [meetingRegistration](../resources/meetingregistration.md) 对象关联的自定义注册问题。

> [!TIP]
> 创建会议注册时，可以按照行创建自定义注册问题。 有关详细信息，请参阅 [创建 meetingRegistration](meetingRegistration-post.md)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetings.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/{id}/registration/microsoft.graph.meetingRegistration/customQuestions
```

> [!TIP]
> 若要访问 `/customQuestions` ，请按照 [示例](#example)将注册类型强制转换到 **meetingRegistration**。

## <a name="request-headers"></a>请求标头

| 名称            | 说明               |
| :-------------- | :------------------------ |
| Authorization   | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [meetingRegistrationQuestion](../resources/meetingregistrationquestion.md) 对象的可写属性的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [meetingRegistrationQuestion](../resources/meetingregistrationquestion.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create-custom-question"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/microsoft.graph.meetingRegistration/customQuestions
Content-Type: application/json

{
  "displayName": "What's your job position?",
  "isRequired": false,
  "answerInputType": "text"
}
```

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "create-custom-question",
  "@odata.type": "microsoft.graph.meetingRegistrationQuestion"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/microsoft.graph.meetingRegistration/customQuestions/$entity",
  "id": "MSNhYjc5NWI4MC119zX3gwMDIwX3lvdXJfeDAwMjBfam8=",
  "displayName": "What's your job position?",
  "isRequired": false,
  "answerInputType": "text",
  "answerOptions": []
}
```
