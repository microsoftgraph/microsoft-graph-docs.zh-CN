---
title: workloadStatus 资源类型
description: 表示工作负荷的状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 50cbd9cdc59426f413333835c4418112401d8038
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402381"
---
# <a name="workloadstatus-resource-type"></a>workloadStatus 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示工作负荷的状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|工作负荷显示名称的负载。 必填。 只读。|
|offboardedDateTime|DateTimeOffset|工作负荷从载出的日期和时间。 可选。 只读。|
|onboardedDateTime|DateTimeOffset|载入工作负荷的日期和时间。 可选。 只读。|
|onboardingStatus|workloadOnboardingStatus|工作负荷的载入状态。 可取值为：`notOnboarded`、`onboarded`、`unknownFutureValue`。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadStatus",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "displayName": "String",
  "offboardedDateTime": "String (timestamp)"
}
```
