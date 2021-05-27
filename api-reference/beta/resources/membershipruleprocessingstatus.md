---
title: membershipRuleProcessingStatus 资源类型
description: 表示动态组处理的当前状态。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7c86f044517ad7b808db69364413727c8d76f076
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680995"
---
# <a name="membershipruleprocessingstatus-resource-type"></a>membershipRuleProcessingStatus 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示动态组处理的当前状态。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| 状态 | [membershipRuleProcessingStatusDetails](#membershipruleprocessingstatusdetails-values) | 动态组处理的当前状态。 可能的值是 `NotStarted` `Running` `Succeeded` ：、、、 `Failed` 和 `UnknownFutureValue` 。  <br><br> 必需。 只读。|
| lastMembershipUpdated | edm。DateTime | 更新动态组的成员身份的最近日期和时间。 <br><br> 可选。 只读。|
| errorMessage | String | 动态组处理出现错误时的详细错误消息。 <br><br> 可选。 只读。|

### <a name="membershipruleprocessingstatusdetails-values"></a>membershipRuleProcessingStatusDetails 值

| 成员 | 说明 |
|:-------- |:----------- |
| NotStarted | 已创建或更新组，并等待处理。|
| 正在运行 | 处理已开始。|
| Succeeded | 处理已完成。 增量对象更改将永久处理。 |
| 已失败 | 处理出现错误。 有关详细信息 **，请参阅 errorMessage。** |
| UnknownFutureValue | 支持未来值。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.membershipRuleProcessingStatus",
  "baseType": null
}-->

```json
{
  "status": "string",
  "lastMembershipUpdated": "DateTime",
  "errorMessage": "string"
}
```
