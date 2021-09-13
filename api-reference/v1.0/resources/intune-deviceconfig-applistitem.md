---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 33d3bf8bed569921016c131ea6d25aeba2f6a924
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019340"
---
# <a name="applistitem-resource-type"></a>appListItem 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




