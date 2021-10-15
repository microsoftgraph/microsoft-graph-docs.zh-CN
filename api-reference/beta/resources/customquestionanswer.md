---
title: customQuestionAnswer 资源类型
description: 表示注册人对自定义注册问题的回答。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/30/2021
doc_type: resourcePageType
ms.openlocfilehash: 4bed8b0c706f7ed1391465534213e849a9f0effe
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369482"
---
# <a name="customquestionanswer-resource-type"></a>customQuestionAnswer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示注册人对与[meetingRegistration](meetingregistration.md)关联的自定义注册问题的回答。 [](meetingregistrationquestion.md)

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| displayName | String | 自定义注册问题的显示名称。 只读。 |
| questionId | String | ID 自定义注册问题。 只读。|
| value | String | 回答自定义注册问题。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customQuestionAnswer"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "value": "String"
}
```
