---
title: deviceManagementExchangeDeviceClass 资源类型
description: 设备中的设备Exchange。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27f74ea0e26fc5f5371bdc864cb4da3c4730c31910b8b1ec366c571eecfa6ade
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178848"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>deviceManagementExchangeDeviceClass 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备中的设备Exchange。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|受此规则影响的设备类的名称。|
|type|[deviceManagementExchangeAccessRuleType](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|受此规则影响的设备类型，例如型号、系列。 可取值为：`family`、`model`。|

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




