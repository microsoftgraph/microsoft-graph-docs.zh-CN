---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8f39b4b93f2551bf89d41faf737d9d3dbfbe5d6
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66722689"
---
# <a name="iosnetworkusagerule-resource-type"></a>iosNetworkUsageRule 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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





