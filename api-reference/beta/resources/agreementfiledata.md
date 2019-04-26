---
title: agreementFileData 资源类型
description: 表示 azure Active Directory (azure AD) 使用条款协议文件的 blob。
localization_priority: Normal
ms.openlocfilehash: c6f4b6708493c0063928a81c95eeb60b7e7603b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339137"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 azure Active Directory (azure AD) 使用条款协议文件的 blob。

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
