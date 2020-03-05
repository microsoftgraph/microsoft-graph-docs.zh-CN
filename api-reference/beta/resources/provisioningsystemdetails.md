---
title: provisioningSystemDetails 资源类型
description: 表示用户预配或来自的系统。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 286ae448cbbaee428820d274d11d8584a9150393
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521318"
---
# <a name="provisioningsystemdetails-resource-type"></a>provisioningSystemDetails 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户预配或来自的系统。 例如，在将用户从 Azure Active Directory （Azure AD）设置为 ServiceNow 时，源系统为 Azure AD，目标系统为 ServiceNow。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|详细信息|[detailsInfo](detailsinfo.md)|系统的详细信息。|
|displayName|String|用户预配或来自的系统的名称。|
|id|String|用户预配或来自的系统的标识符。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystemDetails",
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
  "description": "provisioningSystemDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
