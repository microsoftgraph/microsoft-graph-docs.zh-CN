---
title: businessFlowTemplate 资源类型
description: 在 Azure AD 中访问审阅功能，`businesFlowTemplate`代表 Azure AD 业务流程模板。 创建访问检查时，将呼叫者提供模板，如查看来宾组的成员的标识符。
ms.openlocfilehash: 8faf1a1381f5cdcf4bfaab78adc7a6554479b427
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048210"
---
# <a name="businessflowtemplate-resource-type"></a>businessFlowTemplate 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](accessreviews-root.md)功能中，`businesFlowTemplate`代表 Azure AD 业务流程模板。 创建访问检查时，将呼叫者提供模板，如查看来宾组的成员的标识符。

全局管理员 onboards 租户用于访问审阅功能时，将自动生成的业务流程模板对象。  可以不创建任何其他业务流程模板。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md)集合| 获取业务流程模板相应访问 reviews （英文）。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | 业务流程模板的功能指派的标识符                                      |
| `displayName`            |`String`                | 业务流程模板的名称                                                             |


## <a name="relationships"></a>Relationships

无。

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新 accessReview。 |


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

<!-- {
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
