---
title: recommendedAction 资源类型
description: 表示基于攻击模拟和培训计划的租户建议操作，以改进其安全状况。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8932b20e38da6f544f9f9e668b8b304f49fbde6c
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979483"
---
# <a name="recommendedaction-resource-type"></a>recommendedAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示基于攻击模拟和培训计划的租户建议操作，以改进其安全状况。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionWebUrl|字符串|建议操作的网站 URL。|
|potentialScoreImpact|双精度|建议操作对租户的安全分数有潜在改进。|
|title|String|建议操作的标题。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recommendedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recommendedAction",
  "actionWebUrl": "String",
  "title": "String",
  "potentialScoreImpact": "Double"
}
```

