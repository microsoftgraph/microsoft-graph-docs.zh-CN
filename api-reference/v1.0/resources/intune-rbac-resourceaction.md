---
title: resourceAction 资源类型
description: 资源允许和不允许的操作集。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0ed370ad21ebd913fc9076cc2fbd1629940dd2f83f25a5afabf3207d4a613233
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235427"
---
# <a name="resourceaction-resource-type"></a>resourceAction 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

资源允许和不允许的操作集。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedResourceActions|字符串集合|允许的操作|
|notAllowedResourceActions|字符串集合|不允许的操作。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




