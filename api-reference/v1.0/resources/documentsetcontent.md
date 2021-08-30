---
author: swapnil1993
title: documentSetContent 资源类型
description: documentSetContent 资源包含有关内容的默认内容位置中的文件的元数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5926e80c6c507591942009ae00ea199fdccfdca0
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696566"
---
# <a name="documentsetcontent-resource-type"></a>documentSetContent 资源类型

命名空间：microsoft.graph

表示文档中文档集的默认SharePoint。
## <a name="properties"></a>属性

| 属性名称  | 类型    | 说明|
|:---------------|:--------|:--------------------------------------------------|
| contentType    | microsoft.graph.contentTypeInfo | 文件的内容类型信息。 |
| fileName      | string  | 资源文件夹中应作为默认内容或文档集模板添加的文件的名称。|
| folderName         | string  | 在库中新建文档集时放置文件的文件夹名称。|

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