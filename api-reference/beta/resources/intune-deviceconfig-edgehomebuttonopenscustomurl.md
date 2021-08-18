---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示"开始"按钮;单击"开始"按钮加载特定 URL。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e61160451a7e3c5d72c1cb389cbbf78aa5bd760cd127ab2435b088cb8f32b32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54209915"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a>edgeHomeButtonOpensCustomURL 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

显示"开始"按钮;单击"开始"按钮加载特定 URL。


继承自 [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)

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




