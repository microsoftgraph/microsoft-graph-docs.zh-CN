---
title: workbookCommentReply 资源类型
description: WorkbookCommentReply 资源类型的定义
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 77402ad1566bcfa6822a326270306f1ea604896f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446728"
---
# <a name="workbookcommentreply-resource-type"></a>workbookCommentReply 资源类型

命名空间： microsoft. graph

表示对 Excel 注释的答复。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 workbookCommentReplies](../api/workbookcomment-list-replies.md) | [workbookCommentReply](workbookcommentreply.md)集合 | 检索 workbookcommentreply 对象的列表。 |
| [获取 workbookCommentReply](../api/workbookcommentreply-get.md) | [workbookCommentReply](workbookcommentreply.md) | 读取 workbookCommentReply 对象的属性和关系。 |
| [创建 workbookCommentReply](../api/workbookcomment-post-replies.md) | [workbookCommentReply](workbookcommentreply.md) | 创建新的 workbookCommentReply。 |
## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|内容|String|批注答复的内容。|
|contentType|String|指示批注答复的类型。|
|id|字符串|表示批注标识符。 只读。|


## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
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
  "description": "workbookCommentReply resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
