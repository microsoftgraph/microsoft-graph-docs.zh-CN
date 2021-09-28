---
title: 安全资源类型
description: 连接 Microsoft 安全产品、服务和合作伙伴以简化安全操作并改进威胁防护、检测和响应功能。
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9f4640acb574c5099d0c1e928452099047f9cc71
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979567"
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
|securityactions|[securityAction](../resources/securityaction.md)|响应警报以阻止恶意活动的操作。|
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

