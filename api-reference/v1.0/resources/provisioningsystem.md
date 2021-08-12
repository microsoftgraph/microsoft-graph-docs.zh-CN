---
title: provisioningSystem 资源类型
description: 表示用户已预配到或来自的系统。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 4676a5010b71b7bec5ab01350bb84a69b9dd00158c6622bf208e82a479fab868
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184513"
---
# <a name="provisioningsystem-resource-type"></a>provisioningSystem 资源类型

命名空间：microsoft.graph


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


