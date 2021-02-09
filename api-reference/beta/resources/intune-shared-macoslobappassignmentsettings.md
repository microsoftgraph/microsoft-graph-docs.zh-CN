---
title: macOsLobAppAssignmentSettings 资源类型
description: 包含用于将 Mac LOB 应用分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e00019e2ed7609aa02fc3f16b2076027617fcab
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160544"
---
# <a name="macoslobappassignmentsettings-resource-type"></a>macOsLobAppAssignmentSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于将 Mac LOB 应用分配给组的属性。


继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|uninstallOnDeviceRemoval|布尔|从 Intune 中删除设备时是否卸载应用。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsLobAppAssignmentSettings",
  "uninstallOnDeviceRemoval": true
}
```




