---
title: numberRange 资源类型
description: 号码范围定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 772ffc59bc9ac4848b6b34eee8c62f8006468784
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958716"
---
# <a name="numberrange-resource-type"></a>numberRange 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

号码范围定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lowerNumber|Int32|较小的数字。|
|upperNumber|Int32|上限数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```





