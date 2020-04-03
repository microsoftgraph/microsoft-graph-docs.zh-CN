---
title: businessFlowTemplate 资源类型
description: 在 Azure AD access 评论功能中， `businesFlowTemplate`表示 azure ad 业务流模板。 模板的标识符（如审阅组的来宾成员）是由呼叫者在创建访问评审时提供的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: a8f2d7a876c389d86373f608187f310c515f9cd1
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124425"
---
# <a name="businessflowtemplate-resource-type"></a>businessFlowTemplate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [access 评论](accessreviews-root.md)功能中， `businesFlowTemplate`表示 azure ad 业务流模板。 模板的标识符（如审阅组的来宾成员）是由呼叫者在创建访问评审时提供的。

当全局管理员 onboards 租户使用访问评论功能时，将自动生成业务流模板对象。  业务流模板包括对应用程序的工作分配的访问审核、组成员身份、Azure AD 角色的成员、组的来宾用户成员资格和应用程序的来宾用户分配。 无法创建其他业务流模板。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md)集合| 获取适用于访问评审的业务流模板。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | 功能分配的业务流模板标识符。 这些值区分大小写。                                      |
| `displayName`            |`String`                | 业务流模板的名称                                                             |


## <a name="relationships"></a>关系

无。

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新的 accessReview。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
