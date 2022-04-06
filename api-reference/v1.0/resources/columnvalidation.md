---
author: swapnil1993
title: columnValidation 资源类型
description: 包含验证列值的数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 41136c74347e0acdfe41b5b8fd9a5ddc1501a08b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757848"
---
# <a name="columnvalidation-resource-type"></a>columnValidation 资源类型

命名空间：microsoft.graph

表示验证列值的属性。
## <a name="properties"></a>属性

| 属性  | 类型    | Description|
|:---------------|:--------|:--------------------------------------------------|
| **formula**    | string  | 用于验证列值的公式。 有关示例，请参阅 [列表中常用公式的示例](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3)。|
| **说明**    | 集合 (microsoft.graph.displayNameLocalization)   | 解释此列的值被视为有效的所需值的本地化邮件。 验证失败时，用户收到此消息的提示。 |
| **defaultLanguage**    | string  | 说明的默认 BCP 47 语言标记。|

SharePoint 公式使用一种类似于 Excel 公式的语法。
有关详细信息，请参阅列表[的常用公式SharePoint示例][SPFormulas]。

## <a name="json-representation"></a>JSON 表示形式

下面是 **columnValidation** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnValidation"} -->

```json
{
  "formula": "string",
  "descriptions": [{ "@type": "microsoft.graph.displayNameLocalization" }],
  "defaultLanguage": "string"
}
```

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3
