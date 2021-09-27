---
title: actionResultPart 资源类型
description: 批量操作模型响应的抽象类型。
author: abshar-teams
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fb09088bfdd298d286447b63453f1965f38a9e6a
ms.sourcegitcommit: 30fca91ed203a9ab7b0562833ce0c20c7fb7b7b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/27/2021
ms.locfileid: "59932059"
---
# <a name="actionresultpart-resource-type"></a>actionResultPart 资源类型

命名空间：microsoft.graph

作为批量操作响应模型的基础的抽象类型。 error 属性根据响应是否表示错误进行选择性填充。

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:---------------|:--------|:----------|
|error|[publicError](publicerror.md) |在批量操作过程中发生的错误（如果有）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.actionResultPart"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.actionResultPart",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  }
}
```
## <a name="see-also"></a>另请参阅

- [将成员批量添加到团队](../api/conversationmembers-add.md)

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "actionResultPart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


