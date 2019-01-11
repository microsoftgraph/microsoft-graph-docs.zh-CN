---
title: plannerPlanContextDetailsCollection 资源类型
description: " 值是 plannerPlanContextDetails 对象。"
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 0020ff8e8fd0d2e8dfd783e282e2bd648c16ec6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828236"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>plannerPlanContextDetailsCollection 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。


**PlannerPlanContextDetailsCollection**资源表示的外部上下文计划链接到的集合。 此资源是开放的类型， [plannerPlanDetails](plannerplandetails.md)对象的一部分。 中的属性值对的属性名称是上下文; 特定于应用程序的标识符值是[plannerPlanContextDetails](plannerplancontextdetails.md)对象。


## <a name="properties"></a>属性
打开类型的属性可定义由客户端。 在这种情况下，客户应使用的独特的标识符值，该值代表外部上下文与属性名称。 属性值必须是[plannerPlanContextDetails](plannerplancontextdetails.md)对象。 基于 OData，在打开的类型的属性名称不能包含下列字符： `.`， `:`， `@`， `%`。 需要 URL 编码格式编码这些字符。 在收藏夹列表中删除项目，需要的值从集合中删除[plannerPlanContextCollection](plannerplancontextcollection.md)相反，其自动将此对象中删除的项。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
