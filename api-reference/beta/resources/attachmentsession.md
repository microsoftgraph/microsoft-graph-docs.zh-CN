---
title: attachmentSession 资源类型
description: 表示将大型附件上传到 todoTask 的资源。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 71be9f9afb61735341f98e77b7790b724fcd036a
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645617"
---
# <a name="attachmentsession-resource-type"></a>attachmentSession 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示将大型附件上传到 [todoTask](../resources/todotask.md) 的资源。

继承自 [entity](../resources/entity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|content|流|上传的内容流。|
|expirationDateTime|DateTimeOffset| 上传会话到期时的 UTC 日期和时间。 在此过期时间之前必须上载完整的文件文件。|
|id|String|附件会话的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|nextExpectedRanges|String collection|指示一个值，该值 `{start}` 表示文件中应开始下一次上传的位置。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachmentSession",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentSession",
  "content": "Stream",
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "nextExpectedRanges": [
    "String"
  ]
}
```

