---
title: '已弃用 (businessFlowTemplate 资源类型) '
description: 在 Azure AD 访问评审功能中，表示 `businesFlowTemplate` Azure AD 业务流模板。 创建访问评审时，调用方会提供模板的标识符，例如查看组的来宾成员。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: cfcb1cdc6997cb9b09f2f94a603a2a70c1aaf9d9
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821020"
---
# <a name="businessflowtemplate-resource-type-deprecated"></a>已弃用 (businessFlowTemplate 资源类型) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

在 Azure AD [访问评审](accessreviews-root.md) 功能中， **businesFlowTemplate** 表示 Azure AD 业务流模板。 创建访问评审时，调用方会提供模板的标识符，例如查看组的来宾成员。

当全局管理员载入租户以使用访问评审功能时，将自动生成业务流模板对象。  业务流模板包括对应用程序分配的访问评审、组成员身份、Azure AD 角色的成员身份、组的来宾用户成员身份以及应用程序的来宾用户分配。 无法创建其他业务流模板。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md) 集合| 获取适合访问评审的业务流模板。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| id                     |String                | 业务流模板的功能分配标识符。 这些值区分大小写。                                      |
| displayName            |String                | 业务流模板的名称                                                             |


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


