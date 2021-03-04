---
author: swapnil1993
title: documentSetContent 资源类型
description: documentSetContent 资源包含有关存在于内容的默认内容位置中的文件的元数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8597dfb8a762d2166a9253fb4e806b9c2fcf5223
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446161"
---
# <a name="documentsetcontent-resource-type"></a>documentSetContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
包含有关存在于内容类型的默认内容位置中的文件的元数据。

## <a name="properties"></a>属性

| 属性名称  | 类型    | 说明
|:---------------|:--------|:--------------------------------------------------
| contentType    | microsoft.graph.contentTypeInfo | 文件的内容类型信息。 
| fileName      | string  | 资源文件夹中应添加为默认内容或文档集模板的文件的名称  
| folderName         | string  | 在库中新建文档集时将放置文件的文件夹名称。

## <a name="json-representation"></a>JSON 表示形式

下面是 **documentSetContent** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```