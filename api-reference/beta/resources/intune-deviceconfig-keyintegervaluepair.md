---
title: keyIntegerValuePair 资源类型
description: 带字符串键和整数值的键值对。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0acd0301b50f588197e4eeb40b55ded85d6e26150972ef6d40ecc85c7605b096
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54203034"
---
# <a name="keyintegervaluepair-resource-type"></a>keyIntegerValuePair 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带字符串键和整数值的键值对。


继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|Key|字符串|键值对的字符串键。 继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|
|值|Int32|键值对的整数值。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyIntegerValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyIntegerValuePair",
  "key": "String",
  "value": 1024
}
```




