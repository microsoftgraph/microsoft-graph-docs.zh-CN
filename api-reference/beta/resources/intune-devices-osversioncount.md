---
title: osVersionCount 资源类型
description: 包含每个 OS 版本的包含恶意软件的设备的计数
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa6c8c117fa7cfb9f131d00cff1fe55a21be37ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941770"
---
# <a name="osversioncount-resource-type"></a>osVersionCount 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含每个 OS 版本的包含恶意软件的设备的计数

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|osVersion|String|OS 版本|
|deviceCount|Int32|包含 OS 版本的恶意软件的设备计数|
|lastUpdateDateTime|DateTimeOffset|以 UTC 表示的设备计数的最后更新的时间戳|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```




