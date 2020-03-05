---
title: agreementFileData 资源类型
description: 表示 Azure Active Directory （Azure AD）使用条款协议文件的 blob。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8758de3282bb59220423632be0be9c6e035c18b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508364"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory （Azure AD）使用条款协议文件的 blob。

## <a name="properties"></a>属性
| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|data|Binary|代表使用条款的 PDF 文档的数据。 只读。|

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
