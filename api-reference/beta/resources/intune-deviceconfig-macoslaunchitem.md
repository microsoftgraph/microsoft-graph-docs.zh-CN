---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f432d3ea12a8338c343bce61dcc7a6b2d71ebbef2de70b912d0fb3870fc9d904
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244986"
---
# <a name="macoslaunchitem-resource-type"></a>macOSLaunchItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 macOS 启动项列表中的应用

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|路径|String|启动项的路径。|
|hide|布尔值|是否隐藏用户和组列表中的项目。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```




