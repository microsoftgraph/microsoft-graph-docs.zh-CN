---
title: deviceManagementEnumValue 资源类型
description: 枚举值的定义信息
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9fdddac077caa15fec5cbd516930747ef948665a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777989"
---
# <a name="devicemanagementenumvalue-resource-type"></a>deviceManagementEnumValue 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

枚举值的定义信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|value|String|原始枚举值文本|
|displayName|String|此枚举值的显示名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumValue",
  "value": "String",
  "displayName": "String"
}
```





