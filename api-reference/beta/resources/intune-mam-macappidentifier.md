---
title: macAppIdentifier 资源类型
description: Mac 应用的标识符。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4ee44dc2fe288d7a1605660ef95dc7d88f600fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160521"
---
# <a name="macappidentifier-resource-type"></a>macAppIdentifier 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Mac 应用的标识符。


继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bundleId|String|应用的标识符，如应用商店中指定。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macAppIdentifier",
  "bundleId": "String"
}
```




