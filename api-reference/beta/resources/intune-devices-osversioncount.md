---
title: osVersionCount 资源类型
description: 对每个操作系统版本设备的恶意软件的计数
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de841e679ede22492d26f2a1587e775179c45761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911838"
---
# <a name="osversioncount-resource-type"></a>osVersionCount 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

对每个操作系统版本设备的恶意软件的计数
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|osVersion|String|操作系统版本|
|deviceCount|Int32|设备的操作系统版本恶意软件的计数|
|lastUpdateDateTime|DateTimeOffset|上次更新的设备的时间戳计数以 UTC|

## <a name="relationships"></a>Relationships
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





