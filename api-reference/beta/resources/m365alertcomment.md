---
title: m365AlertComment 资源类型
description: 与警报或事件相关联的分析员生成的注释。
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c3c59422a8e379bbe7ecf43890774a9474d51b26
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220836"
---
# <a name="m365alertcomment-resource-type"></a>m365AlertComment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与警报或事件相关联的分析员生成的注释。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|注释|String|批注文字。|
|createdByDisplayName|字符串|提交评论的人或应用名称。|
|createdDateTime|DateTimeOffset|提交注释的时间。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.m365AlertComment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.m365AlertComment",
  "comment": "String",
  "createdByDisplayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

