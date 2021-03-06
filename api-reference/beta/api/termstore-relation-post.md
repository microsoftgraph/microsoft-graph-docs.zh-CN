---
title: 创建关系
description: 创建新的关系对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: da7d01377a31c74d7f2adbbfa1f5df7452c62d91
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872301"
---
# <a name="create-relation"></a>创建关系
命名空间：microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [关系](../resources/termstore-relation.md) 对象。 它们用于创建术语之间或术语和集之间的固定和重复使用关系。 在术语和设置之间创建固定/重复使用的术语时，post 正文中的 fromTerm 必须为 null。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） |TermStore.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供关系对象的 JSON [表示](../resources/termstore-relation.md) 形式。

下表显示创建关系时所需的 [属性](../resources/termstore-relation.md)。

|属性|类型|Description|
|:---|:---|:---|
|关系|relationType|要创建的关系的类型。 可取值为：`pin`、`reuse`。|
|set| [microsoft.graph.termstore.set](../resources/termstore-set.md)| 需要创建关系的集。
|fromTerm| [microsoft.graph.termstore.term](../resources/termstore-term.md) | 需要创建关系的术语。



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回响应代码[](../resources/termstore-relation.md)和 relation 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}/relations
Content-Type: application/json
Content-length: 89

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "relationship": "pin",
  "fromTerm" : {
    "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "set" : {
    "id": "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.relation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "052c749c-749c-052c-9c74-2c059c742c05",
  "relationship": "pin",
  "fromTerm" : {
      "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "toTerm" : {
      "id" : "226e8ee3-f4b6-49d7-92d5-ec9d5475eec5"
  },
  "set" : {
      "id" : "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Pinned term",
  "suppressions": [
  ]
}
-->


