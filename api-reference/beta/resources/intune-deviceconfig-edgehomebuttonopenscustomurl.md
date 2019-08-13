---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c3fa2465200b216e3519b4eb15700406bd67f16
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332545"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a>edgeHomeButtonOpensCustomURL 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。


继承自[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|homeButtonCustomURL|String|要加载的特定 URL。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```



