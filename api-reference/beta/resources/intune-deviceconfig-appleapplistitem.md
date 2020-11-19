---
title: appleAppListItem 资源类型
description: 表示托管 Apple 应用程序列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a95905ef8076883ebdeea4a5ea6973017e511fee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283747"
---
# <a name="appleapplistitem-resource-type"></a>appleAppListItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示托管 Apple 应用程序列表中的应用程序


继承自 [appListItem](../resources/intune-deviceconfig-applistitem.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|name|字符串|从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序名称|
|发布者|String|从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序的发布者|
|appStoreUrl|String|继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)的应用程序的存储 URL|
|appId|String|从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序的应用程序或捆绑包标识符|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




