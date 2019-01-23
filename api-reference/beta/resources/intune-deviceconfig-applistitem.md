---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9571b622fc098f384f7c3a6c62b1d1e10d89f663
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405413"
---
# <a name="applistitem-resource-type"></a>appListItem 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示托管应用程序列表中的应用

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|应用程序名称|
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




