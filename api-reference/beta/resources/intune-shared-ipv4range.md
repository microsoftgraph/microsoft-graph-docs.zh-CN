---
title: iPv4Range 资源类型
description: IP V4 范围
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a1f76fcd99663fe7ddd34263c8304b5597e6941c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888289"
---
# <a name="ipv4range-resource-type"></a>iPv4Range 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

IP V4 范围

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
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



