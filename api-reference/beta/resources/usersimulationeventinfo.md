---
title: userSimulationEventInfo 资源类型
description: 表示攻击模拟和培训活动中租户中用户的模拟事件。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 423eb3f5f15d4730d1229febde71aec9930ff81f
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979480"
---
# <a name="usersimulationeventinfo-resource-type"></a>userSimulationEventInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训活动中租户中用户的模拟事件。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|浏览器|字符串|用户在攻击模拟和培训活动中发起模拟事件的浏览器信息。|
|eventDateTime|DateTimeOffset|用户在攻击模拟和培训活动中的模拟事件的日期和时间。|
|eventName|字符串|攻击模拟和培训活动中用户模拟事件的名称。|
|ipAddress|String|用户在攻击模拟和培训活动中启动模拟事件的 IP 地址。|
|osPlatformDeviceDetails|字符串|用户从其中启动模拟事件（在攻击模拟和培训活动中）的操作系统、平台和设备详细信息。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSimulationEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSimulationEventInfo",
  "eventName": "String",
  "eventDateTime": "String (timestamp)",
  "ipAddress": "String",
  "osPlatformDeviceDetails": "String",
  "browser": "String"
}
```

