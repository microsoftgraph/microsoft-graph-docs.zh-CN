---
title: agreementFileData 资源类型
description: 表示Azure Active Directory (Azure AD) 使用条款协议文件。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 25d24851827b469bf7b6a6d121e1ba92bd79b0b0
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451366"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData 资源类型

命名空间：microsoft.graph

表示Azure Active Directory (Azure AD) 使用条款协议文件。

## <a name="properties"></a>属性
| 属性       | 类型 | 说明 |
|:-------------|:------------|:------------|
|data|Binary|表示 PDF 文档的使用条款的数据。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


