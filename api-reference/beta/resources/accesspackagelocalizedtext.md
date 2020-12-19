---
title: accessPackageLocalizedText 资源类型
description: 用于表示特定语言中的字符串的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9573ae4118f02abdba5686fd94da96da71d374c2
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720134"
---
# <a name="accesspackagelocalizedtext-resource-type"></a>accessPackageLocalizedText 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于表示特定语言中的字符串的复杂类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|languageCode|String|目标语言的 ISO 代码。 必需。 |
|text|String|特定语言的文本。 必填。 |

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
