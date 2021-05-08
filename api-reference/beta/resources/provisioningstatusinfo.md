---
title: provisioningStatusInfo 资源类型
description: 描述预配摘要事件的状态。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 669201b5527160da6b903614523d633a8c11cb1d
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232916"
---
# <a name="provisioningstatusinfo-resource-type"></a>provisioningStatusInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述预配摘要事件的状态。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|状态|String| 可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。|
|errorInfo|[provisioningErrorInfo](provisioningerrorinfo.md)| 如果状态未成功/跳过错误的详细信息将包含在其中。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
  "baseType": null
}-->

```json
{
  "status": "String",
  "errorinfo": {"@odata.type": "microsoft.graph.provisioningErrorInfo"},}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStatusInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


