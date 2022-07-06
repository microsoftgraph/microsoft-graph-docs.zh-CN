---
title: taskFileAttachment 资源类型
description: 表示附加到 todoTask 的文件（如文本文件或 Word 文档）。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1724222d362edae4f053af58ce52680052a15be7
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645634"
---
# <a name="taskfileattachment-resource-type"></a>taskFileAttachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示附加到 [todoTask](../resources/todotask.md) 的文件（如文本文件或 Word 文档）。
在任务上创建文件附件时，包括 `"@odata.type": "#microsoft.graph.taskFileAttachment"` 属性 **名称** 和 **contentBytes**。

继承自 [attachmentBase](../resources/attachmentbase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出附件](../api/todotask-list-attachments.md)|[taskFileAttachment](../resources/taskfileattachment.md) 集合|获取 [taskFileAttachment](../resources/taskfileattachment.md) 对象及其属性的列表。|
|[创建附件](../api/todotask-post-attachments.md)|[taskFileAttachment](../resources/taskfileattachment.md) 集合|将新的 [taskFileAttachment](../resources/taskfileattachment.md) 对象添加 [到 todoTask](../resources/todotask.md)。|
|[创建上传会话](../api/taskfileattachment-createuploadsession.md)|[taskFileAttachment](../resources/taskfileattachment.md) 集合|创建上传会话，以迭代方式将文件范围作为附件上传到 [todoTask](../resources/todotask.md)。|
|[获取附件](../api/taskfileattachment-get.md)|[taskFileAttachment](../resources/taskfileattachment.md)|读取 [taskFileAttachment](../resources/taskfileattachment.md) 对象的属性和关系。|
|[删除附件](../api/taskfileattachment-delete.md)|无|删除 [taskFileAttachment](../resources/taskfileattachment.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentBytes|Binary|文件的 Base64 编码内容。|
|contentType|String|附件的内容类型。 继承自 [attachmentBase](../resources/attachmentbase.md)。|
|id|字符串|附件的 ID。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。 继承自 [attachmentBase](../resources/attachmentbase.md)。|
|name|String|在表示嵌入附件的图标下显示的文本的名称。 这不必是实际的文件名。 继承自 [attachmentBase](../resources/attachmentbase.md)。|
|size|Int32|附件大小，以字节为单位。 继承自 [attachmentBase](../resources/attachmentbase.md)。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taskFileAttachment",
  "baseType": "microsoft.graph.attachmentBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "contentBytes": "Binary",
  "contentType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": "Int32"
}
```

