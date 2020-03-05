---
title: workbookComment 资源类型
description: 代表工作簿中的注释。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c2165f43c04ebbaf3274cc0ae912756bf250785a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519244"
---
# <a name="workbookcomment-resource-type"></a>workbookComment 资源类型

命名空间： microsoft. graph

代表工作簿中的注释。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 workbookComments](../api/workbook-list-comments.md) | [workbookComment](workbookComment.md)集合 | 获取**workbookComment**对象集合。 |
| [获取 workbookComment](../api/workbookcomment-get.md) | [workbookComment](workbookcomment.md) | 读取**workbookComment**对象的属性和关系。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|内容|String|注释的内容。|
|contentType|String|指示注释的类型。|
|id|字符串| 表示批注标识符。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|应答|[workbookCommentReply](workbookcommentreply.md)集合| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "content": "String",
  "contentType": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookComment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
