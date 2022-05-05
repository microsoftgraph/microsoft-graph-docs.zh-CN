---
title: androidDeviceOwnerUserFacingMessage 资源类型
description: 表示面向用户的消息，其中包含区域设置信息，以及在用户的区域设置与任何本地化消息不匹配时要使用的默认消息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07e57975a7aadf6e0d0dfe0b7479b66ef0c01d47
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213191"
---
# <a name="androiddeviceowneruserfacingmessage-resource-type"></a>androidDeviceOwnerUserFacingMessage 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示面向用户的消息，其中包含区域设置信息，以及在用户的区域设置与任何本地化消息不匹配时要使用的默认消息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|localizedMessages|[keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md) 集合|<区域设置的列表，消息>对。 该集合最多可包含 500 个元素。|
|defaultMessage|String|如果用户的区域设置与任何本地化消息不匹配，则显示默认消息|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerUserFacingMessage",
  "localizedMessages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "defaultMessage": "String"
}
```




