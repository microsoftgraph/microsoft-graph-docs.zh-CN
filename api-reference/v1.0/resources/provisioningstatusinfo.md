---
title: provisioningStatusInfo 资源类型
description: 描述预配摘要事件的状态。
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 82b13a700cece9b558ec131f68ea3f79fc0105c2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052872"
---
# <a name="provisioningstatusinfo-resource-type"></a>provisioningStatusInfo 资源类型

命名空间：microsoft.graph


描述预配摘要事件的状态。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|状态|provisioningResult| 可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。|
|errorInfo|[provisioningErrorInfo](provisioningErrorInfo.md)| 如果状态未成功/跳过错误的详细信息将包含在其中。|

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
  "status": "String"
}
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


