---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4174f6f8dbd1a94ce3246189683529a9fdb4346927465b3f084fb77974313992
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163752"
---
# <a name="printsettings-resource-type"></a>printSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示通用打印服务的租户范围设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|documentConversionEnabled|Boolean|指定是否对租户启用文档转换。 如果启用文档转换，通用打印服务将自动将文档转换为与打印机兼容的格式 (xps) pdf 格式。|

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

