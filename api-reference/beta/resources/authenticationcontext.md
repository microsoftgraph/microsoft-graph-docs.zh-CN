---
title: authenticationContext 资源类型
description: 描述登录事件的条件访问身份验证上下文。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c768615d585423f2dd99c95961965d415bde1244
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137238"
---
# <a name="authenticationcontext-resource-type"></a>authenticationContext 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述登录事件的条件访问身份验证上下文。 

有关条件访问中的身份验证上下文的更多详细信息，请参阅条件 [访问上下文文档](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#authentication-context-preview)。 

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|detail|authenticationContextDetail|介绍如何触发条件访问身份验证上下文。 值 表示身份验证上下文是因为用户已在以前的一些身份验证事件满足该身份验证 `previouslySatisfied` 上下文的要求。 值 表示用户必须满足身份验证上下文要求作为登录流程的一 `required` 部分。 可能的值包括 `required`、`previouslySatisfied`、`notApplicable`、`unknownFutureValue`。|
|id|String|租户中身份验证上下文的标识符。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationContext"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationContext",
  "id": "String (identifier)",
  "detail": "String"
}
```

