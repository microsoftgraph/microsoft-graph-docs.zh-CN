---
title: accessPackageLocalizedContent 资源类型
description: 用于表示不同区域设置中的文本以及默认文本的复杂类型。*
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91ef87428b4171317943e9ecf1ec92e959c7a62b
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720116"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a>accessPackageLocalizedContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于表示多个本地化窗体中的文本的复杂类型。 它包含一个默认文本，在请求的本地化不可用时，会使用该文本。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|defaultText|String|回退字符串，在请求的本地化不可用时使用。 必需。 |
|localizedTexts|[accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md) 集合|以特定区域设置的格式表示的内容。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedContent",
  "defaultText": "String",
  "localizedTexts": [
    {
      "@odata.type": "microsoft.graph.accessPackageLocalizedText"
    }
  ]
}
```
