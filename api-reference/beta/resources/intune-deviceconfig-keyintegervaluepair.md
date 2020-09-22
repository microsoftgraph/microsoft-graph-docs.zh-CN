---
title: keyIntegerValuePair 资源类型
description: 带有字符串键和整数值的键-值对。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efba214d6cd6b4e8fb79ddb4df4c9df0e16974bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092543"
---
# <a name="keyintegervaluepair-resource-type"></a>keyIntegerValuePair 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带有字符串键和整数值的键-值对。


继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|Key|字符串|键/值对的字符串键。 继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|
|值|Int32|键/值对的整数值。|

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






