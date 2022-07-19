---
title: 安全资源类型
description: 连接 Microsoft 安全产品、服务和合作伙伴，以简化安全操作并改进威胁防护、检测和响应功能。
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c7342f83c64b895b08a66429e0e20ab2cd7b5960
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856286"
---
# <a name="security-resource-type"></a>安全资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

连接 Microsoft 安全产品、服务和合作伙伴，以简化安全操作并改进威胁防护、检测和响应功能。

## <a name="methods"></a>方法
无。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|警报|[警报](../resources/alert.md)集合|有关客户租户中可疑或潜在安全问题的通知。|
|attackSimulation|[attackSimulationRoot](../resources/attacksimulationroot.md)|提供租户功能，以启动模拟和逼真的网络钓鱼攻击并从中学习。|
|securityactions|[securityAction](../resources/securityaction.md)|响应警报以阻止恶意活动的操作。|
|tiindicators|[tiIndicator](../resources/tiindicator.md) 集合|发送到 Microsoft 的威胁指示器，用于识别恶意活动。|
|threatSubmission|[security.threatSubmission](../resources/security-threatsubmission.md)|发送给 Microsoft 的威胁提交;例如，可疑的电子邮件威胁、URL 威胁或文件威胁。|

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

