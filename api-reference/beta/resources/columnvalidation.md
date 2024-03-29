---
author: swapnil1993
title: columnValidation 资源类型
description: 包含用于验证列值的数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 20bf526aff4f10b0b9b16a31e9912b5695602db6
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63721722"
---
# <a name="columnvalidation-resource-type"></a>columnValidation 资源类型

命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
包含用于验证列的元数据。

## <a name="properties"></a>属性

| 属性            | 类型                                                | 说明                                                                                                                                                                                                               |
| :------------------ | :-------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **formula**         | string                                              | 用于验证列值的公式。 有关示例，请参阅 [列表中常见公式的示例](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3) |
| **说明**    | 集合 (microsoft.graph.displayNameLocalization)  | 解释此列的值被视为有效的所需值的本地化邮件。 验证失败时，用户收到此消息的提示。                                                               |
| **defaultLanguage** | string                                              | 说明的默认 BCP 47 语言标记。                                                                                                                                                                          |

SharePoint 公式使用一种类似于 Excel 公式的语法。
有关详细信息[，请参阅 SharePoint 列表中常见][SPFormulas]公式的示例。

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
