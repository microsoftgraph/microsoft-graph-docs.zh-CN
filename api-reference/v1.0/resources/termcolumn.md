---
author: swapnil1993
title: termColumn 资源类型
description: 术语Column 资源指示列的值包含分类数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 38fa6fe4fdb7b08f93287305e43dddb4ec6d9331
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696548"
---
# <a name="termcolumn-resource-type"></a>termColumn 资源类型

命名空间：microsoft.graph

表示托管元数据列中SharePoint。

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明|
|:--------------|:-------|:----------------------------------------------------|
| allowMultipleValues | 布尔值 | 指定列是否允许多个值。|
| parentTerm     | microsoft.graph.termStore.term | 指定可选择其子项作为列值的术语 GUID。  |
| showFullyQualifiedName | 布尔值 | 指定是显示整个术语路径还是仅显示术语标签。  |
| termSet      | microsoft.graph.termStore.set | 可以选择其子项作为列值的术语集。 |

## <a name="json-representation"></a>JSON 表示形式

下面是 **termColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```

