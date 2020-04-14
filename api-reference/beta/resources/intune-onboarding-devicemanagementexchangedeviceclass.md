---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4099009c67e2c5b0ce8cc5b3c52dd00b1fd32aec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448041"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>deviceManagementExchangeDeviceClass 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Exchange 中的设备类。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|将受此规则影响的设备类别的名称。|
|type|[deviceManagementExchangeAccessRuleType](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|受此规则影响的设备类型，例如 Model、Family。 可取值为：`family`、`model`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```



