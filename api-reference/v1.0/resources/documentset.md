---
author: swapnil1993
title: documentSet 资源类型
description: 包含有关文档集设置的元数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 9edfe45791f3fa0c9404c7418e3c0a2f647d9c2c
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758199"
---
# <a name="documentset-resource-type"></a>documentSet 资源类型

命名空间：microsoft.graph

表示文档中的文档SharePoint。

## <a name="properties"></a>属性

| 属性  | 类型    | Description|
|:---------------|:--------|:--------------------------------------------------|
| allowedContentTypes | 集合 (microsoft.graph.contentTypeInfo)  | 文档集允许的内容类型。|
| defaultContents     | 集合 (microsoft.graph.documentSetContent)  | 文档集的默认内容。 | 
| propagateWelcomePageChanges | Boolean | 指定是否将欢迎页面更改推送到继承的内容类型。  |
| shouldPrefixNameToFile | Boolean  | 指示是否将文档集的名称添加到每个文件名。 |
| welcomePageUrl      | string | 欢迎页面绝对 URL。  |

## <a name="relationships"></a>关系

| 关系   | 类型                      | Description
|:----------------|:--------------------------|:-------------------------------
| sharedColumns       | 集合 (microsoft.graph.columnDefinition)  | 在同步到文档集内所有文档的文档集上编辑的列。 这些文档本身是只读的。 
| welcomePageColumns  | 集合 (microsoft.graph.columnDefinition)   | 指定要显示在文档集的欢迎页上的列。

## <a name="json-representation"></a>JSON 表示形式

下面是 **documentSet** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
