---
title: attachmentInfo 资源类型
description: 表示附件的属性。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: af43c3e53dd41a28f9e123912bf6153679500f00
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645619"
---
# <a name="attachmentinfo-resource-type"></a>attachmentInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示附件的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|attachmentType|attachmentType|附件的类型。 可能的值包括 `file`、`item`、`reference`。 必需。|
|contentType|String|附件中数据的性质。 可选。|
|name|String|附件的显示名称。 这可以是描述性字符串，不必是实际的文件名。 必需。|
|size|Int64|附件大小，以字节为单位。 必填。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attachmentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentInfo",
  "attachmentType": "String",
  "contentType": "String",
  "name": "String",
  "size": "Int64"
}
```

