---
title: publicInnerError 资源类型
description: 表示错误的内部详细信息。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d0d14ffb803a084db080dc986ceb0dc83f14619dd3230b68aacf07401f13543
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139114"
---
# <a name="publicinnererror-resource-type"></a>publicInnerError 资源类型

命名空间：microsoft.graph

表示 [publicError 的内部详细信息](../resources/publicerrordetail.md)。 
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|code|String|错误代码。|
|详细信息|[publicErrorDetail](../resources/publicerrordetail.md) 集合|错误详细信息的集合。|
|message|String|错误消息。|
|target|String|错误的目标值。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicInnerError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicInnerError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ]
}
```

