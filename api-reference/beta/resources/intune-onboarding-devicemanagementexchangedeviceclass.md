---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e512253a9b9bc4228d41c369501bec1e7a5e031
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413729"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>deviceManagementExchangeDeviceClass 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Exchange 中的设备类。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|设备类，该类将会受到此规则的名称。|
|type|[deviceManagementExchangeAccessRuleType](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|设备受到此规则的类型例如建模、 系列。 可取值为：`family`、`model`。|

## <a name="relationships"></a>Relationships
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




