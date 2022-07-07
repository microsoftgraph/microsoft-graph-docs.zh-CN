---
title: conditionalAccessApplications 资源类型
description: 表示策略范围中包含和排除的应用程序和用户操作。
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b7c92b9eab03adb284fdde95794c45fc4f7be19d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668074"
---
# <a name="conditionalaccessapplications-resource-type"></a>conditionalAccessApplications 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示条件访问策略中包含和排除的应用程序和用户操作。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| includeApplications | 字符串集合 | 可以是下列类型之一： <li> 应用策略) **appId** (客户端 ID 列表，除非在 **excludeApplications** 中显式排除 ()  <li> `All` <li> `Office365`- 有关包含在其中`Office365`的应用列表，请[参阅条件访问目标应用：Office 365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps) |
| excludeApplications | 字符串集合 | 可以是下列类型之一： <li>  (**appId**) 显式排除在策略中的客户端 ID 列表。<li> `Office365`- 有关包含在其中`Office365`的应用列表，请[参阅条件访问目标应用：Office 365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps) |
| includeUserActions | 字符串集合 | 要包含的用户操作。 支持的值为 `urn:user:registersecurityinfo` 和 `urn:user:registerdevice` |
| includeAuthenticationContextClassReferences | 字符串集合 | 身份验证上下文类引用包括。 支持的值是 `c1` 通过 `c25`。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

