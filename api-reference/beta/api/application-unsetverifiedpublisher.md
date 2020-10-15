---
title: 应用程序： unsetVerifiedPublisher
description: 取消设置应用程序的已验证发布者。
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1f904a4b13e162dc503765b03d676319d3d0a510
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471549"
---
# <a name="application-unsetverifiedpublisher"></a>应用程序： unsetVerifiedPublisher

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

取消设置之前在[应用程序](../resources/application.md)上设置的[verifiedPublisher](../resources/verifiedPublisher.md) ，并删除所有已验证的发布服务器属性。 有关详细信息，请参阅 [Publisher 验证](/azure/active-directory/develop/publisher-verification-overview)。

## <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持 |
|应用程序 | 不支持 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a>请求标头

| 名称           | 说明                |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/unsetVerifiedPublisher
```

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: b0ed721f-7e6a-446c-89bc-2d03e1744dfe
2020-09-09 21:26:11 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: unsetVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
