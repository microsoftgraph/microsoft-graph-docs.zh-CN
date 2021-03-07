---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 53e0db2a1923cad0af1f35baf5bed6fecd896fb3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516987"
---
# <a name="printsettings-resource-type"></a>printSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示通用打印服务的租户范围设置。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|documentConversionEnabled|Boolean|指定是否对租户启用文档转换。 如果启用文档转换，通用打印服务将自动将文档转换为与打印机兼容格式， (xps) pdf 格式。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printSettings",
  "documentConversionEnabled": "Boolean"
}
```

