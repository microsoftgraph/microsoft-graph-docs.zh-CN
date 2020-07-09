---
title: 删除 taskDefinition
description: 删除任务定义。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 23d7438d573cb0ac8ff17c0a9c100bece71bb68c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091648"
---
# <a name="delete-taskdefinition"></a>删除 taskDefinition

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除**taskDefinition**。

有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="permissions"></a>权限
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| 不支持。 |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| PrintTaskDefinition |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/taskDefinitions/{id}
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}. Required. |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "delete_taskdefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19
```

---

### <a name="response"></a>响应
下面展示了示例响应。
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
