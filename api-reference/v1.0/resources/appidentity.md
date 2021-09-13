---
title: appIdentity 资源类型
description: 指示执行该操作或已更改的应用程序的标识。 包括应用程序 ID、名称、服务主体 ID 和名称。 此资源由 directoryAudit API 调用
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8259ab10f798e3e50d9d7eaec5fbd9aecb3719df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062815"
---
# <a name="appidentity-resource-type"></a>appIdentity 资源类型

命名空间：microsoft.graph

指示执行该操作或已更改的应用程序的标识。 包括应用程序 ID、名称和服务主体 ID 和名称。 此资源由 Get [directoryAudit 操作](../api/directoryaudit-get.md) 使用。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appId|String|表示唯一 GUID（表示 Azure Active Directory 中的应用程序 ID）。|
|displayName|String|引用 Azure 门户中显示的应用程序名称。|
|servicePrincipalId|String|指相应应用的唯一 GUID，Azure Active Directory服务主体 ID。|
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

