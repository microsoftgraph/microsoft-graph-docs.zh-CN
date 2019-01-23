---
title: osVersionCount 资源类型
description: 对每个操作系统版本设备的恶意软件的计数
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbe0d8ac149ad84ba4cd1286fb0f2303cdfb52a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410460"
---
# <a name="osversioncount-resource-type"></a>osVersionCount 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对每个操作系统版本设备的恶意软件的计数

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|osVersion|String|操作系统版本|
|deviceCount|Int32|设备的操作系统版本恶意软件的计数|
|lastUpdateDateTime|DateTimeOffset|上次更新的设备的时间戳计数以 UTC|

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




