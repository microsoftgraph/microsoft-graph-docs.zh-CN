---
title: 发起者资源类型
description: 描述发起预配事件的人或发起者。
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5a00be289964c749adcea2b7f4df80dd477c1a99
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129857"
---
# <a name="initiator-resource-type"></a>发起者资源类型

命名空间：microsoft.graph

描述发起预配事件的人或发起者。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|发起预配事件的人员或服务的名称。|
|id|String|唯一标识发起预配事件的人员或服务。|
|initiatorType|initiatorType| 发起人的类型。 可取值为：`user`、`application`、`system`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


