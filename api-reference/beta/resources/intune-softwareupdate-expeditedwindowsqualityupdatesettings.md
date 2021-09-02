---
title: expeditedWindowsQualityUpdateSettings 资源类型
description: 用于存储快速质量更新设置（如发布日期和强制重启前天数）的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 55328cb788ab1994eec2ec7e0f8984577b7b9a3b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805273"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a>expeditedWindowsQualityUpdateSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于存储快速质量更新设置（如发布日期和强制重启前天数）的复杂类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|qualityUpdateRelease|String|用于标识质量更新的发布日期。|
|daysUntilForcedReboot|Int32|安装后将发生强制重启的天数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expeditedWindowsQualityUpdateSettings",
  "qualityUpdateRelease": "String",
  "daysUntilForcedReboot": 1024
}
```



