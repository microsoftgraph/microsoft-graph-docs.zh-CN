---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40d1631264f1aaaab5483cecd08222bb969c8a48
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447043"
---
# <a name="macoslaunchitem-resource-type"></a>macOSLaunchItem 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 macOS 启动项列表中的应用程序

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|路径|String|启动项目的路径。|
|选中|Boolean|是否要从 "用户和组" 列表中隐藏项目。|

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



