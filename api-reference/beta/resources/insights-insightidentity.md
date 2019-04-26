---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8718ab248dada75f04d92d6a8717dd4f43ee8106
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333594"
---
# <a name="insightidentity"></a>insightIdentity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含[共享](insights-shared.md)项目的属性的复杂类型。 

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
| displayName       | 字符串          | 共享项目的用户的显示名称。 |
| id              | String        | 共享项的用户的 id。     |
| address             | String      | 共享项目的用户的电子邮件地址。  |
