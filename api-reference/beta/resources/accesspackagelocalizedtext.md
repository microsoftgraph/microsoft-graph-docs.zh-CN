---
title: accessPackageLocalizedText 资源类型
description: 用于表示特定语言中的字符串的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8d493f0909617dcda26546ccc262d7591c6b9309
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137345"
---
# <a name="accesspackagelocalizedtext-resource-type"></a>accessPackageLocalizedText 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于表示特定语言中的字符串的复杂类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|languageCode|字符串|目标语言的 ISO 代码。 必填。 |
|text|字符串|特定语言的文本。 必填。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedText",
  "text": "String",
  "languageCode": "String"
}
```
