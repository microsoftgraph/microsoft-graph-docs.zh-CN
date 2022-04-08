---
title: 删除 delegatedAdminRelationship
description: 删除 delegatedAdminRelationship 对象。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 41087bde23bfba8bdf2f5ec969bdd13f80c69f1f
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704373"
---
# <a name="delete-delegatedadminrelationship"></a>删除 delegatedAdminRelationship
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [delegatedAdminRelationship](../resources/delegatedadminrelationship.md) 对象。 仅当关系处于"已创建"状态时，才能删除关系。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|If-Match|If-match： {etag}。 要删除的 **delegatedAdminRelationship** 的最后一个已知 ETag 值。 从 LIST 或 GET 操作中检索 ETag 值。 必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "delete_delegatedadminrelationship"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836
If-Match: W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="
```


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

