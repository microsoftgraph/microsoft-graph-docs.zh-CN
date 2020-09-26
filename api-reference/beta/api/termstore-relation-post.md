---
title: 创建关系
description: 创建新的 relation 对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8c44856d97ceb0986e6cab71d4be4d0ef62ee0b6
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288691"
---
# <a name="create-relation"></a>创建关系
命名空间： termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [relation](../resources/termstore-relation.md) 对象。 这些关系用于在术语之间或术语和 set 之间创建固定的和重用的关系。 在术语和 set 之间创建固定/重用术语时，在帖子正文中 fromTerm 必须为 null。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
在请求正文中，提供 [relation](../resources/termstore-relation.md) 对象的 JSON 表示形式。

下表显示创建 [关系](../resources/termstore-relation.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|关系|relationType|要创建的关系类型。 可取值为：`pin`、`reuse`。|
|set| [termstore 设置](../resources/termstore-set.md)| 需要在其中创建关系的集合。
|fromTerm| [microsoft termstore](../resources/termstore-term.md) | 需要创建关系的术语。



## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [relation](../resources/termstore-relation.md) 对象。

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


