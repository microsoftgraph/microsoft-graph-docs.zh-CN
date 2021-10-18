---
title: continuousAccessEvaluationSessionControl 资源类型
description: 用于控制连续访问评估设置的会话控制。
author: lujiangfeng666
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: caa6c09d54d2305af348b848d99e0e43049f5c55
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450789"
---
# <a name="continuousaccessevaluationsessioncontrol-resource-type"></a>continuousAccessEvaluationSessionControl 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于控制连续访问评估设置的会话控制。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|mode|continuousAccessEvaluationMode| 指定连续访问评估设置。 可能的值包括 `strictEnforcement`、`disabled`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationSessionControl"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationSessionControl",
  "mode": "String"
}
```
