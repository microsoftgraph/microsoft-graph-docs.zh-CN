---
title: conditionalAccessRoot 资源类型
description: conditionalAccessRoot 资源是条件访问 (CA) 入口点。 它不包含任何可用属性。
ms.localizationpriority: medium
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 739b02a5bf06c7ac742b524e406145c29bb40aa3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59110511"
---
# <a name="conditionalaccessroot-resource-type"></a>conditionalAccessRoot 资源类型

命名空间：microsoft.graph

**conditionalAccessRoot** 资源是 CA (条件访问) 入口点。 它不包含任何可用属性。

有关条件访问中条件访问Azure Active Directory，请参阅[什么是条件访问](/azure/active-directory/conditional-access/overview)？

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|namedLocations|[namedLocation](namedlocation.md) 集合| 只读。 可为空。 返回指定命名位置的集合。|
|策略|[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合| 只读。 可为空。 返回指定的条件访问或 CA 策略 (一) 集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessRoot"
}-->

```json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot"
}
```