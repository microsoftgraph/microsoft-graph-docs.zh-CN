---
title: userTrainingStatusInfo 资源类型
description: 表示分配的培训及其在攻击模拟和培训中的用户状态。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: d9e2900bb2c72ba8100d5fe49130b7229db988ee
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757841"
---
# <a name="usertrainingstatusinfo-resource-type"></a>userTrainingStatusInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示分配的培训及其在攻击模拟和培训中的用户状态。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|assignedDateTime|DateTimeOffset|向用户分配培训的日期和时间。|
|completionDateTime|DateTimeOffset|用户完成培训的日期和时间。|
|displayName|String|已分配培训的显示名称。|
|trainingStatus|trainingStatus|分配给用户的培训的状态。 可取值为：`unknown`、`assigned`、`inProgress`、`completed`、`overdue`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingStatusInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingStatusInfo",
  "assignedDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "trainingStatus": "String",
  "displayName": "String"
}
```

