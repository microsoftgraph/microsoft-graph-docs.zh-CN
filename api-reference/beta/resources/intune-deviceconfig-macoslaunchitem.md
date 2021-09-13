---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c000ac1bb9240eaad505a6d50d34b58cba4dc13a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146679"
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
|hide|Boolean|是否隐藏用户和组列表中的项目。|

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



