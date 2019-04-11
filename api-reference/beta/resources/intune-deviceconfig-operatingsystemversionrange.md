---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80b0afb706a71ef8e0e3d4877fa7d0df822fe1d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788119"
---
# <a name="operatingsystemversionrange-resource-type"></a>operatingSystemVersionRange 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

操作系统版本范围。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|此范围的说明 (例如, 有效的1702版本)|
|lowestVersion|String|此范围包含的最低包含版本。|
|highestVersion|String|此范围包含的最高包含版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





