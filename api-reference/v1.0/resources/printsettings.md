---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围设置。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 11cba611772065f8c2014143f0c83b45eb6bd766
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944261"
---
# <a name="printsettings-resource-type"></a>printSettings 资源类型

命名空间：microsoft.graph

表示通用打印服务的租户范围设置。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|documentConversionEnabled|Boolean|指定是否对租户启用文档转换。 如果启用文档转换，通用打印服务将自动将文档转换为与打印机兼容的格式， (xps) pdf 格式。|

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

