---
title: userTrainingStatusInfo 资源类型
description: 表示分配的培训及其在攻击模拟和培训中的用户状态。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 82b0c6b1de49c9b8eb0572dab33fca8c90e2b6fe
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979548"
---
# <a name="usertrainingstatusinfo-resource-type"></a>userTrainingStatusInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示分配的培训及其在攻击模拟和培训中的用户状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignedDateTime|DateTimeOffset|向用户分配培训的日期和时间。|
|completionDateTime|DateTimeOffset|用户完成培训的日期和时间。|
|displayName|字符串|已分配培训的显示名称。|
|trainingStatus|trainingStatus|分配给用户的培训的状态。 可取值为：`unknown`、`assigned`、`inProgress`、`completed`、`overdue`、`notCompleted`、`unknownFutureValue`。|

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

