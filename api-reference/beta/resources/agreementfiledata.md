---
title: agreementFileData 资源类型
description: 代表 Azure Active Directory 的 blob (Azure AD) 使用条款使用协议文件。
localization_priority: Normal
ms.openlocfilehash: 64de3a72ad648225f24429987f5729f76ed8a2e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815215"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表 Azure Active Directory 的 blob (Azure AD) 使用条款使用协议文件。

## <a name="properties"></a>属性
| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|data|Binary|表示使用 PDF 文档中的条款的数据。 此为只读属性。|

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
