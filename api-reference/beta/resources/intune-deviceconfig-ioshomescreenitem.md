---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 077c0eea7a4953d0cba3e9223a24fd9107f1b6c0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990251"
---
# <a name="ioshomescreenitem-resource-type"></a>iosHomeScreenItem 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 iOS 主屏幕上的项

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|应用的名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





