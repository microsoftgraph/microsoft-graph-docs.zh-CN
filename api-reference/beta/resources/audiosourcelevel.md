---
title: audioSourceLevel 资源类型
description: 对于其他源的级别配置。
author: VinodRavichandran
ms.openlocfilehash: 5d5abe7eba03891427b30ba1c8f63b15b3707e46
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380238"
---
# <a name="audiosourcelevel-resource-type"></a>audioSourceLevel 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

对于其他源的级别配置。

## <a name="properties"></a>属性

| 属性               | 类型    | 说明                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | Boolean | 允许此源回避活动时的其他源。 如果设置为 true，放掉级别设置。|
| level                  | Int64   | 如果放掉源的级别`duckOthers`设置为`true`。                                     |
| 参与者            | 字符串  | 源参与者音频流。                                                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
