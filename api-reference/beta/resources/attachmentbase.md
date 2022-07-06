---
title: attachmentBase 资源类型
description: 表示附件的抽象基类型。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 355492402cd8532098ef81618c6407c0ba7f167a
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645626"
---
# <a name="attachmentbase-resource-type"></a>attachmentBase 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示附件的抽象基类型。 可以以附件的形式将相关内容添加 [到 todoTask](../resources/todotask.md) 。

[taskFileAttachment](../resources/taskfileattachment.md) 的基本类型。

继承自 [entity](../resources/entity.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentType|String|MIME 类型。|
|id|String|附件的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|name|String|附件的显示名称。 这不必是实际的文件名。|
|size|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachmentBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentBase",
  "contentType": "String",  
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": "Int32"
}
```

