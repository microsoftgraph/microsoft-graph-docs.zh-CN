---
title: informationProtectionContentLabel 资源类型
description: 介绍在对象上定义 MIP 元数据的 informationProtectionContentLabel 对象。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4f615655110ffdc6b76469d3d29cd4d13663d511
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938826"
---
# <a name="informationprotectioncontentlabel-resource-type"></a>informationProtectionContentLabel 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍在对象上定义 MIP 元数据的 informationProtectionContentLabel 对象。 **informationProtectionContentLabel**由[extractLabel](../api/informationprotectionlabel-extractLabel.md) API 返回到当前应用于文件的标签。 

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|assignmentMethod|字符串| 可取值为：`standard`、`privileged`、`auto`。|
|creationDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|label|[labelDetails](labeldetails.md)| 当前应用于文件的标签上的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.informationProtectionContentLabel",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "creationDateTime": "String (timestamp)",
  "label": {"@odata.type": "microsoft.graph.labelDetails"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionContentLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->