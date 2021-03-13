---
title: auditLogRoot 资源类型
description: 包含不同类型的审核日志。 此资源返回单一的 auditLog 资源。 它不包含任何可用属性。
author: dhanyahk
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 363d3a0c3aafbbd5b3d53914748dfdb1fd432b1b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759725"
---
# <a name="auditlogroot-resource-type"></a>auditLogRoot 资源类型

命名空间：microsoft.graph

包含不同类型的审核日志。 此资源返回单一的 auditLog 资源。 它不包含任何可用属性。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |列出集合中的目录审核项及其属性。|
|[获取 directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |获取特定目录审核项及其属性。|
|[列出 signIn](../api/signin-list.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|
|[获取 signIn](../api/signin-get.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|directoryAudits|[directoryAudit](directoryaudit.md) 集合| 只读。 可为 NULL。|
|signIns|[signIn](signin.md) 集合| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.auditLogRoot"
}-->

```json
{
}
```

## <a name="example"></a>示例


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-auditlogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditLogRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

