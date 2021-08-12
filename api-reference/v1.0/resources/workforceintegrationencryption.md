---
title: workforceIntegrationEncryption 资源类型
description: 定义员工集成的协议和密码的加密实体。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a05111fb561fe806b8b590eef321e3b7fcc9ebcd9054d2d8e5f7853e6d0c88b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180451"
---
# <a name="workforceintegrationencryption-resource-type"></a>workforceIntegrationEncryption 资源类型

命名空间：microsoft.graph

定义员工重新参与的协议和密码的 [加密实体](../resources/workforceintegration.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|协议|String| 可取值为：`sharedSecret`、`unknownFutureValue`。|
|secret|String|加密共享密码。|

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

