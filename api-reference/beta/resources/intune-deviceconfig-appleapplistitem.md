---
title: appleAppListItem 资源类型
description: 表示托管 Apple 应用程序列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4804f3834a63a3c446c09d383c2244def97398
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470123"
---
# <a name="appleapplistitem-resource-type"></a>appleAppListItem 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示托管 Apple 应用程序列表中的应用程序


继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|字符串|从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序名称|
|发布者|String|从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序的发布者|
|appStoreUrl|String|继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)的应用程序的存储 URL|
|appId|String|继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)的应用程序的捆绑包标识符|

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



