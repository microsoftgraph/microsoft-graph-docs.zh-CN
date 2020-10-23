---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b1d5aa08940f4d49ecb0c78f6c81aa358c578a44
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701464"
---
# <a name="macoslaunchitem-resource-type"></a>macOSLaunchItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 macOS 启动项列表中的应用程序

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|路径|String|启动项目的路径。|
|选中|布尔|是否要从 "用户和组" 列表中隐藏项目。|

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





