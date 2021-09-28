---
title: userTrainingContentEventInfo 资源类型
description: 表示在攻击模拟和培训活动中向用户分配的培训的培训计划详细信息。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2771c9924bcd0d3441e404b37f7aa75ec55e9c91
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979556"
---
# <a name="usertrainingcontenteventinfo-resource-type"></a>userTrainingContentEventInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训活动中的培训计划的详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|浏览器|字符串|生成培训计划的用户的浏览器。|
|contentDateTime|DateTimeOffset|用户播放培训内容的日期和时间。|
|ipAddress|String|培训活动的用户的 IP 地址。|
|osPlatformDeviceDetails|字符串|用户用于培训课程的操作系统、平台和设备详细信息。|
|potentialScoreImpact|双精度|用户完成培训后租户安全状态的潜在改进。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingContentEventInfo",
  "contentDateTime": "String (timestamp)",
  "ipAddress": "String",
  "osPlatformDeviceDetails": "String",
  "browser": "String",
  "potentialScoreImpact": "Double"
}
```

