---
title: businessFlowTemplate 资源类型
description: 在 Azure AD 访问评审功能中，表示 `businesFlowTemplate` Azure AD 业务流程模板。 模板的标识符（如查看组的来宾成员）由调用方在创建访问评审时提供。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: b1fce9de1c2f21d4a5c918985028acfee50dc390
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751242"
---
# <a name="businessflowtemplate-resource-type"></a>businessFlowTemplate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [访问评审](accessreviews-root.md) 功能中 **，businesFlowTemplate** 表示 Azure AD 业务流程模板。 模板的标识符（如查看组的来宾成员）由调用方在创建访问评审时提供。

当全局管理员载入租户以使用访问评审功能时，将自动生成业务流程模板对象。  业务流程模板包括对应用程序的分配的访问评审、组的成员身份、Azure AD 角色的成员身份、组的来宾用户成员身份以及到应用程序的来宾用户分配。 无法创建其他业务流程模板。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md) 集合| 获取适用于访问评论的业务流程模板。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| id                     |String                | 业务流程模板的功能分配标识符。 这些值区分大小写。                                      |
| displayName            |String                | 业务流程模板的名称                                                             |


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


