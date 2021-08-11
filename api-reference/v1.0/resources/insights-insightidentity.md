---
title: insightIdentity
description: 包含共享项的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 393a6c1f7fbd1a7fffac667afcf054cdc6b54d55576ffb220df6437166827622
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229254"
---
# <a name="insightidentity"></a>insightIdentity

命名空间：microsoft.graph

包含 [sharedInsight 项的属性的复杂](insights-shared.md) 类型。 

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>属性

| 属性              | 类型          | 说明  |
| -------------         |-----------    | -------------|
| displayName       | String          | 共享显示名称的用户的行数。 |
| id              | String        | 共享项的用户的 ID。     |
| address             | String      | 共享项目的用户的电子邮件地址。  |

