---
title: oemWarranty 资源类型
description: 给定设备的 OEM 担保信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e64e0018fc185cfb79ecc32990b6c4ad4b02c7d
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292288"
---
# <a name="oemwarranty-resource-type"></a>oemWarranty 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的 OEM 担保信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|baseWarranties|[warrantyOffer](../resources/intune-devices-warrantyoffer.md) 集合|基本担保产品/服务列表。 此集合最多可包含 100 个元素。|
|additionalWarranties|[warrantyOffer](../resources/intune-devices-warrantyoffer.md) 集合|其他担保产品/服务的列表。 此集合最多可包含 100 个元素。|
|deviceWarrantyUrl|String|设备担保页面 URL|
|deviceConfigurationUrl|String|设备配置页面 URL|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oemWarranty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oemWarranty",
  "baseWarranties": [
    {
      "@odata.type": "microsoft.graph.warrantyOffer",
      "type": "String",
      "description": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)"
    }
  ],
  "additionalWarranties": [
    {
      "@odata.type": "microsoft.graph.warrantyOffer",
      "type": "String",
      "description": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)"
    }
  ],
  "deviceWarrantyUrl": "String",
  "deviceConfigurationUrl": "String"
}
```




