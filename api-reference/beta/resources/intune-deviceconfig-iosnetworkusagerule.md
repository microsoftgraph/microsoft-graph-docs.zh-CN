---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a287fcf8be771037a39efd821f5468acf518371
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398322"
---
# <a name="iosnetworkusagerule-resource-type"></a>iosNetworkUsageRule 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|managedApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|要应用此规则的托管应用的相关信息。 该集合最多可包含 500 个元素。|
|cellularDataBlockWhenRoaming|Boolean|如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。|
|cellularDataBlocked|Boolean|如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```




