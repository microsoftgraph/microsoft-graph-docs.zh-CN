---
title: workforceIntegrationEncryption 资源类型
description: 为劳动力集成定义协议和密码的加密实体。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 15feb2097a3a7bf36092070cc2af4841d2aa3839
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019392"
---
# <a name="workforceintegrationencryption-resource-type"></a>workforceIntegrationEncryption 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为 [workforceintegration](../resources/workforceintegration.md)定义协议和密码的加密实体。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|协议|String| 可取值为：`sharedSecret`、`unknownFutureValue`。|
|私钥|String|加密共享密钥。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
  "baseType": null
}-->

```json
{
  "protocol": "String",
  "secret": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegrationEncryption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


