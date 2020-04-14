---
title: androidManagedStoreAppTrack 资源类型
description: 包含适用于 Android 托管存储应用的跟踪信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d505a11016ae9959ff783e15b83d912346365183
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449784"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a>androidManagedStoreAppTrack 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含适用于 Android 托管存储应用的跟踪信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|trackId|String|唯一的曲目标识符。|
|trackAlias|String|跟踪的友好名称。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppTrack"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppTrack",
  "trackId": "String",
  "trackAlias": "String"
}
```



