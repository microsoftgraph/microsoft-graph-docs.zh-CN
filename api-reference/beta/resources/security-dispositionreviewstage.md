---
title: dispositionReviewStage 资源类型
description: 表示一个多级别审阅过程，审阅者在处置的每个阶段指示是删除还是进一步保留内容项。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: cc89d8c907fcd6ec84c4810f30e19921e6312d1c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447585"
---
# <a name="dispositionreviewstage-resource-type"></a>dispositionReviewStage 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个多级审阅过程，审阅者在处置的每个阶段指示是删除还是进一步保留内容项。
有关详细信息，请参阅 [内容的处置](/microsoft-365/compliance/disposition)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 retentionLabel](../api/security-retentionlabel-post.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|创建新的 [retentionLabel](../resources/security-retentionlabel.md) 对象。 |
|[更新 retentionLabel](../api/security-retentionlabel-update.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|更新 [retentionLabel](../resources/security-retentionlabel.md) 对象。 |


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|每个阶段的唯一 ID。 |
|name|String|表示集合中每个阶段的名称。 |
|reviewersEmailAddresses|String collection|每个阶段的审阅者集合。 |
|stageNumber|Int32|处置评审的每个阶段的序列号。 |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dispositionReviewStage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dispositionReviewStage",
  "id": "String (identifier)",
  "stageNumber": "Integer",
  "name": "String",
  "reviewersEmailAddresses": [
    "String"
  ]
}
```
