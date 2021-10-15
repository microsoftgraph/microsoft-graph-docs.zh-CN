---
title: 删除 meetingRegistration
description: 删除和禁用会议注册。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fae1f288cf8338f419133a3cec9039869b50d956
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369449"
---
# <a name="delete-meetingregistration"></a>删除 meetingRegistration

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表组织者禁用和删除[onlineMeeting](../resources/onlinemeeting.md)的[meetingRegistration。](../resources/meetingregistration.md)

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetings.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onlineMeetings/{id}/registration
```

## <a name="request-headers"></a>请求标头

| 名称            | 说明               |
| :-------------- | :------------------------ |
| Authorization   | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法仅返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "delete-registration"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "delete-registration"
}-->

```http
HTTP/1.1 204 No Content
```
