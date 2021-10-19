---
title: 标识资源类型
description: 标识
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cac61a828f7d602bfd0bb0775e35f323ba0d491e
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60486824"
---
# <a name="identity-resource-type"></a>标识资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

标识

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|标识的标识符。 此属性是只读的。|
|displayName|String|标识显示名称的标识。 此属性是只读的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identity",
  "id": "String (identifier)",
  "displayName": "String"
}
```



