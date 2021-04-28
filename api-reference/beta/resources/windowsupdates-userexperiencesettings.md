---
title: userExperienceSettings 资源类型
description: 设置控制用户对设备的更新体验。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a5d920d1618cb6d212baf0487a39960638859cef
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067257"
---
# <a name="userexperiencesettings-resource-type"></a>userExperienceSettings 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置控制用户对设备的更新体验。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|daysUntilForcedReboot|Int32|指定安装更新后的天数，在此期间设备用户可以控制设备重启的时间。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.userExperienceSettings",
  "daysUntilForcedReboot": "Integer"
}
```

