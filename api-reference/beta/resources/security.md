---
title: 安全资源类型
description: 连接 Microsoft 安全产品、服务和合作伙伴以简化安全操作并改进威胁防护、检测和响应功能。
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 494fc483645fe0a5422013556b2a44cc21aaadaf
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220764"
---
# <a name="security-resource-type"></a>安全资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

连接 Microsoft 安全产品、服务和合作伙伴以简化安全操作并改进威胁防护、检测和响应功能。

## <a name="methods"></a>方法
无。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|警报|[警报](../resources/alert.md)集合|有关客户租户中可疑或潜在安全问题的通知。|
|attackSimulation|[attackSimulationRoot](../resources/attacksimulationroot.md)|为租户提供启动模拟和真实的钓鱼攻击并学习其信息的功能。|
|事件 | [事件](incident.md) 集合 | 事件集中的事件Microsoft 365 Defender，每个事件都是反映攻击事件的一组相关警报和关联元数据。|
|secureScores | [secureScore](securescores.md) 集合 | 租户安全状况的度量，有助于保护他们免受威胁。 |
|securityactions|[securityAction](../resources/securityaction.md) 集合|响应警报以阻止恶意活动的操作。|
|tiindicators|[tiIndicator](../resources/tiindicator.md) 集合|发送给 Microsoft 的威胁指示器，用于标识恶意活动。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security"
}
```

