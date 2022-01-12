---
title: workloadStatus 资源类型
description: 表示工作负荷的状态。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d85d7fd60a269c360185d8d4ffb5952a71bdd628
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792265"
---
# <a name="workloadstatus-resource-type"></a>workloadStatus 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示工作负荷的状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|工作负荷显示名称的负载。 必需。 只读。|
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
