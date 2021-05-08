---
title: provisioningSystem 资源类型
description: 表示用户已预配到或来自的系统。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2dcc52e4b847648477313d61c8b69b168a8807b1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232914"
---
# <a name="provisioningsystem-resource-type"></a>provisioningSystem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户已预配到或来自的系统。 例如，将用户从 Azure Active Directory (Azure AD) ServiceNow 时，源系统是 Azure AD，目标系统是 ServiceNow。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|详细信息|[detailsInfo](detailsinfo.md)|系统的详细信息。|
|displayName|String|用户预配到或来自的系统的名称。|
|id|String|用户预配到或设置自的系统标识符。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystem",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


