---
title: membershipRuleProcessingStatus 资源类型
description: 表示动态组处理的当前状态。
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 592a07abacf15300b25bfa00e9b477f9923d6c25
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64586907"
---
# <a name="membershipruleprocessingstatus-resource-type"></a>membershipRuleProcessingStatus 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示动态组处理的当前状态。

## <a name="properties"></a>属性

| 属性              | 类型                                                                                   | 说明                                                                                                                                                                |
| :-------------------- | :------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 状态                | [membershipRuleProcessingStatusDetails](#membershipruleprocessingstatusdetails-values) | 动态组处理的当前状态。 可能的值是：、`NotStarted``Running`、`Succeeded`、`Failed`和 `UnknownFutureValue`。 <br><br> 必需项。 只读。 |
| lastMembershipUpdated | edm。DateTime                                                                           | 更新动态组的成员身份的最近日期和时间。 <br><br> 可选。 只读。                                                                    |
| errorMessage          | String                                                                                 | 动态组处理出现错误时的详细错误消息。 <br><br> 可选。 只读。                                                                        |

### <a name="membershipruleprocessingstatusdetails-values"></a>membershipRuleProcessingStatusDetails 值

| 成员             | 说明                                                                     |
| :----------------- | :------------------------------------------------------------------------------ |
| NotStarted         | 已创建或更新组，正在等待处理。                     |
| 正在运行            | 处理已开始。                                                         |
| Succeeded          | 处理已完成。 增量对象更改将永久处理。 |
| 已失败             | 处理出现错误。 有关详细信息 **，请参阅 errorMessage** 。                 |
| UnknownFutureValue | 支持未来值。                                                         |

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
