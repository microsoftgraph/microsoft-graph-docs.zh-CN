---
title: appleAppListItem 资源类型
description: 表示托管 Apple 应用程序列表中的应用程序
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 91a43ee845998535331804936becb6596ee7e2bd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075597"
---
# <a name="appleapplistitem-resource-type"></a>appleAppListItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示托管 Apple 应用程序列表中的应用程序


继承自 [appListItem](../resources/intune-deviceconfig-applistitem.md)

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|name|String|应用程序名称 继承自 [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|发布者|String|应用程序的发布者 继承自 [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|appStoreUrl|String|应用程序的应用商店 URL 继承自 [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|appId|String|应用程序的应用程序或捆绑包标识符 继承自 [appListItem](../resources/intune-deviceconfig-applistitem.md)|

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



