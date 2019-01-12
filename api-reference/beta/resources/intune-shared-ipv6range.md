---
title: iPv6Range 资源类型
description: IPV6 范围
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c30d85a83bb604a5c0ccb6563d6315a183f6497
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971478"
---
# <a name="ipv6range-resource-type"></a>iPv6Range 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

IPV6 范围

继承自 [ipRange](../resources/intune-shared-iprange.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lowerAddress|String|IP 地址下限|
|upperAddress|String|IP 地址上限|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



