---
title: managedDeviceModelsAndManufacturers 资源类型
description: 帐户中托管设备型号和制造商的元数据
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1b560cb95766d3216b566d33cfe00db2689c6efd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137796"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>managedDeviceModelsAndManufacturers 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

帐户中托管设备型号和制造商的元数据

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceModels|字符串集合|帐户中托管设备的型号列表|
|deviceManufacturers|字符串集合|帐户中托管设备的制造者列表|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```



