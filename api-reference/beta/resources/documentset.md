---
author: swapnil1993
title: documentSet 资源类型
description: 包含有关文档集设置的元数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 25a2b5e71c76a8a097ff9c490313ae6d319abeb8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446160"
---
# <a name="documentset-resource-type"></a>documentSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
包含有关文档集设置的元数据。

## <a name="properties"></a>属性

| 属性名称  | 类型    | 说明
|:---------------|:--------|:--------------------------------------------------
| shouldPrefixNameToFile | 布尔  | 将文档集的名称添加到每个文件名。
| allowedContentTypes | collection (microsoft.graph.contentTypeInfo)  | 文档集允许的内容类型。
| defaultContents     | 集合 (microsoft.graph.documentSetContent)  | 文档集的默认内容。  
| propagateWelcomePageChanges | 布尔 | 指定是否将欢迎页面更改推送到继承的内容类型。  
| sharedColumns       | 集合 (microsoft.graph.columnDefinition)  | 在同步到文档集内所有文档的文档集上编辑的列。 这些文档本身是只读的。 
| welcomePageColumns  | 集合 (microsoft.graph.columnDefinition)   | 指定要显示在文档集的欢迎页上的列。  
| welcomePageUrl      | string | 欢迎页面绝对 URL。  

## <a name="json-representation"></a>JSON 表示形式

下面是 **documentSet** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "sharedColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
