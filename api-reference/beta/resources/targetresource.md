---
title: targetResource 资源复杂类型 - Microsoft Graph API
description: 定义 Microsoft Graph API 的 targetResource 实体资源复杂类型，该 API 支持审核日志报告 (租户) 活动。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: afcb3ecec2df719393fbadd033b6f1c85af447c9ea901356a71480bc17a67a74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244244"
---
# <a name="targetresource-resource-type"></a>targetResource 资源类型

命名空间：microsoft.graph

表示与审核活动关联的目标资源类型。 


## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String|指示资源的唯一 ID。|
|displayName|字符串|指示为资源定义的可见名称。 通常在创建资源时指定。|
|type|字符串|描述资源类型。  示例值包括 `Application` 、 、 和 `Group` `ServicePrincipal` `User` 。|
|userPrincipalName|String|当 **type** 设置为 `User` 时，这包括启动该操作的用户名; `null` 对于其他类型。|
|groupType|groupType|当 **type** 设置为 `Group` 时，这表示组类型。  可能的值包括 `unifiedGroups` ：、 `azureAD` 和 `unknownFutureValue`|
|ModifiedProperties|[modifiedProperty](modifiedproperty.md) 集合|指示更改的每个属性的名称、旧值和新值。 属性值取决于操作 **类型**。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String", 
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


