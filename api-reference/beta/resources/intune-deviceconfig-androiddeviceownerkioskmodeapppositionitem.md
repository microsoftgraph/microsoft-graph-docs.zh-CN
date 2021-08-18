---
title: androidDeviceOwnerKioskModeAppPositionItem 资源类型
description: 应用位置列表中的项，用于设置托管主屏幕上的项目顺序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4e658e4289f2d08dbb8552bd3496db6d80a9161d5d065d88a11691061340d29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245112"
---
# <a name="androiddeviceownerkioskmodeapppositionitem-resource-type"></a>androidDeviceOwnerKioskModeAppPositionItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

应用位置列表中的项，用于设置托管主屏幕上的项目顺序

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|position|Int32|项目在网格上的位置。 有效值为 0 到 9999999|
|项|[androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)|要排列的项目|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
  "position": 1024,
  "item": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
    "label": "String",
    "link": "String"
  }
}
```




