---
title: chromeOSDeviceProperty 资源类型
description: 表示 ChromeOS 设备的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3746cdd02a3b12ad9c657c1e5377a4b0b02adc47
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818994"
---
# <a name="chromeosdeviceproperty-resource-type"></a>chromeOSDeviceProperty 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 ChromeOS 设备的属性。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|name|String|属性的名称|
|value|String|属性的值|
|valueType|String|值的类型|
|updatable|布尔值|此属性是否可更新|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chromeOSDeviceProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSDeviceProperty",
  "name": "String",
  "value": "String",
  "valueType": "String",
  "updatable": true
}
```



