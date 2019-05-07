---
title: appIdentity 资源类型
description: 指示执行了操作或已更改的应用程序的标识。 包括应用程序 Id、名称、服务主体 ID 和名称。 此资源由 directoryAudit API 调用
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a4e7f5a21d5140537e745f7234186ad3b24098f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629353"
---
# <a name="appidentity-resource-type"></a>appIdentity 资源类型

指示执行了操作或已更改的应用程序的标识。 包括应用程序 ID、名称和服务主体 ID 和名称。 [Get directoryAudit](../api/directoryaudit-get.md)操作使用此资源。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appId|String|表示唯一 GUID（表示 Azure Active Directory 中的应用程序 ID）。|
|displayName|字符串|引用 Azure 门户中显示的应用程序名称。|
|servicePrincipalId|字符串|指在 Azure Active Directory 中指示对应应用程序的服务主体 Id 的唯一 GUID。|
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
