---
title: appIdentity 资源类型
description: 指示执行该操作或已更改的应用程序的标识。 包括应用程序 ID、名称、服务主体 ID 和名称。 此资源由 directoryAudit API 调用
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: sureshja
ms.openlocfilehash: 66a830d5a030a6b3247e3265aaeaa66452a7c577
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336926"
---
# <a name="appidentity-resource-type"></a>appIdentity 资源类型

命名空间：microsoft.graph

指示执行该操作或已更改的应用程序的标识。 此资源由 [directoryAudit](../api/directoryaudit-get.md) API 调用。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appId|String|引用表示应用程序中的应用程序 ID 的唯一Azure Active Directory。|
|displayName|String|引用 Azure 门户中显示的应用程序名称。|
|servicePrincipalId|String|引用指示相应应用的 Azure Active Directory 中服务主体 ID 的唯一标识符。|
|servicePrincipalName|String|引用服务主体名称是租户中的应用程序名称。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


