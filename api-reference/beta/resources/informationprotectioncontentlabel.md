---
title: informationProtectionContentLabel 资源类型
description: 介绍在对象上定义 MIP 元数据的信息ProtectionContentLabel 对象。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b4d113e0f8f6d8f057a93d9094533e7fa2d5be6c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962600"
---
# <a name="informationprotectioncontentlabel-resource-type"></a>informationProtectionContentLabel 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍在对象上定义 MIP 元数据的信息ProtectionContentLabel 对象。 **informationProtectionContentLabel** 由 [extractLabel](../api/informationprotectionlabel-extractLabel.md) API 解析为当前应用于文件的标签返回。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|assignmentMethod|String| 可取值为：`standard`、`privileged`、`auto`。|
|creationDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|label|[labelDetails](labeldetails.md)| 有关当前应用于文件的标签的详细信息。 |

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

