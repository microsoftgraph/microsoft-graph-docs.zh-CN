---
title: simulationAutomation 资源类型
description: 表示为在租户上运行而创建的模拟自动化。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 38f8bf63ef41053666a4bdd58121bd81e09fe51c
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758313"
---
# <a name="simulationautomation-resource-type"></a>simulationAutomation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示为在租户上运行而创建的模拟自动化。


## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 simulationAutomations](../api/attacksimulationroot-list-simulationautomations.md)|[simulationAutomation](../resources/simulationautomation.md) 集合|获取 [simulationAutomation 对象](../resources/simulationautomation.md) 及其属性的列表。|
|[列出运行](../api/simulationautomation-list-runs.md)|[simulationAutomationRun](../resources/simulationautomationrun.md) 集合|获取租户的攻击模拟自动化运行列表。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[emailIdentity](../resources/emailidentity.md)|创建攻击模拟自动化的用户的标识。|
|createdDateTime|DateTimeOffset|创建攻击模拟自动化的日期和时间。|
|description|String|攻击模拟自动化的说明。|
|displayName|String|攻击模拟自动化的显示名称。 支持 `$filter` 和 `$orderby`。|
|id|String|攻击模拟自动化的唯一标识符。|
|lastModifiedBy|[emailIdentity](../resources/emailidentity.md)|最近修改攻击模拟自动化的用户的标识。|
|lastModifiedDateTime|DateTimeOffset|最近修改攻击模拟自动化的日期和时间。|
|lastRunDateTime|DateTimeOffset|最近运行攻击模拟自动化的日期和时间。|
|nextRunDateTime|DateTimeOffset|即将运行的攻击模拟自动化的日期和时间。|
|状态|[simulationAutomationStatus](#simulationautomationstatus-values)|攻击模拟自动化的状态。 支持 `$filter` 和 `$orderby`。 可能的值包括 `unknown`、`draft`、`notRunning`、`running`、`completed`、`unknownFutureValue`。|

### <a name="simulationautomationstatus-values"></a>simulationAutomationStatus 值

|成员|说明 |
|:---|:---|
|unknown| 未定义模拟自动化的状态。 |
|draft| 模拟自动化在草稿模式下。 |
|notRunning| 模拟自动化未运行。 |
|running| 模拟自动化正在运行。 |
|已完成| 模拟自动化已完成。 |
|unknownFutureValue| 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|runs|[simulationAutomationRun](../resources/simulationautomationrun.md) 集合|模拟自动化运行的集合。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulationAutomation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationAutomation",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastRunDateTime": "String (timestamp)",
  "nextRunDateTime": "String (timestamp)",
  "status": "String"
}
```

