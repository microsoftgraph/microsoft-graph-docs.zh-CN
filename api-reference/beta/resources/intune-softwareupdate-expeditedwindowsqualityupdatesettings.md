---
title: expeditedWindowsQualityUpdateSettings 资源类型
description: 用于存储快速质量更新设置（如发布日期和天，直到强制重启）的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 700b86d15737c75cbf10679ea6e944726d667431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160197"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a>expeditedWindowsQualityUpdateSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于存储快速质量更新设置（如发布日期和天，直到强制重启）的复杂类型。

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




