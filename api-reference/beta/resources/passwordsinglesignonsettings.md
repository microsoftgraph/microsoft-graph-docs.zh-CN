---
title: passwordSingleSignOnSettings 资源类型
description: 与基于密码的单一登录相关的设置
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3e7e4402e6416166dd7c288cdd9aa9ec5ecbba06
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761540"
---
# <a name="passwordsinglesignonsettings-resource-type"></a>passwordSingleSignOnSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含基于密码的单一登录设置的集合。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|域|[passwordSingleSignOnField](passwordsinglesignonfield.md) 集合||

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnSettings",
  "baseType": null
}-->

```json
{
  "fields": [{"@odata.type": "microsoft.graph.passwordSingleSignOnField"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

