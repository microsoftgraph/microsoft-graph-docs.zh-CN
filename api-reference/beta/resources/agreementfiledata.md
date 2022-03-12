---
title: agreementFileData 资源类型
description: 表示协议Azure Active Directory (Azure AD) 文件的 blob。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 3fa6c94497ae42b102f03bee6142ec38677eda93
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451310"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示协议Azure Active Directory (Azure AD) 文件的 blob。

## <a name="properties"></a>属性
| 属性       | 类型 | 说明 |
|:-------------|:------------|:------------|
|data|Binary|表示 PDF 文档的使用条款的数据。 只读。 <br/><br/>**注意：** 您可以使用 .NET [Convert.ToBase64String](/dotnet/api/system.convert.tobase64string) 方法，使用创建协议 API 将文件转换为二进制数据 [进行](../api/termsofusecontainer-post-agreements.md) 上载。 在 PowerShell 中使用此方法的示例语法是 `[convert]::ToBase64String((Get-Content -path "your_file_path" -Encoding byte))`。 |

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


