---
title: deviceHealthScriptParameter 资源类型
description: script 参数的基本属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 65102807cee2d369e658f2c0de1ffc9822380015
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59144299"
---
# <a name="devicehealthscriptparameter-resource-type"></a>deviceHealthScriptParameter 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

script 参数的基本属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|参数的名称|
|说明|String|参数的说明|
|isRequired|Boolean|参数是否是必需的|
|applyDefaultValueWhenNotAssigned|Boolean|未分配时是否应用 DefaultValue|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true
}
```



