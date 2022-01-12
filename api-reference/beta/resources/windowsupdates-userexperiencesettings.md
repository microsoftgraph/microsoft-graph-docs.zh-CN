---
title: userExperienceSettings 资源类型
description: 设置控制用户对设备的更新体验。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 889e771f34cc88244f79785cb29c388a88fcd61b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792167"
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

