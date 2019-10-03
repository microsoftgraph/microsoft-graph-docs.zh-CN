---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c43b559f1c1994d34ae0d4202b4970227d029df7
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366739"
---
# <a name="applistitem-resource-type"></a>appListItem 资源类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示托管应用程序列表中的应用

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|字符串|应用程序名称|
|publisher|String|应用程序发布者|
|appStoreUrl|String|应用程序的应用商店 URL|
|appId|String|应用程序或应用程序的捆绑标识符|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




