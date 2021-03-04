---
title: identityUserFlowAttribute 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的用户流属性。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 3e8707627b09784972a1a578fe4b6b84a623f4dd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440239"
---
# <a name="identityuserflowattribute-resource-type"></a>identityUserFlowAttribute 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Azure Active Directory（Azure AD）租户和 Azure AD B2C 租户中的用户流属性。

在 Azure AD 或 Azure AD B2C 租户中配置用户流属性，可在注册期间收集用户的相关信息。 可选择收集内置属性集；例如，指定名字、姓氏、市/县和邮政编码。 还可以配置自定义用户流属性，以便收集未内置到目录中的用户的信息。 自定义用户流属性是对[Azure Active Directory 架构扩展](/azure/active-directory/develop/active-directory-schema-extensions)的抽象。

## <a name="methods"></a>Methods

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identityuserflowattribute-list.md)|identityUserFlowAttributes collection|检索所有内置和自定义的用户流属性。|
|[创建](../api/identityuserflowattribute-post.md)|identityUserFlowAttribute|创建新的自定义用户流属性。|
|[获取](../api/identityuserflowattribute-get.md) |identityUserFlowAttribute|检索用户流属性的属性。|
|[更新](../api/identityuserflowattribute-update.md)|无|更新自定义用户流属性。|
|[删除](../api/identityuserflowattribute-delete.md)|无|删除自定义用户流属性。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|用户流属性的标识符。 这是一个自动创建的只读属性。|
|displayName|String|用户流属性的显示名称。|
|说明|String|注册时显示给用户的用户流量属性的描述。|
|userFlowAttributeType|String|用户流属性的类型。 这是一个自动设置的只读属性。 此属性的值将是 `builtIn` 或 `custom`，具体取决于属性的类型。|
|DataType|String|用户流属性的数据类型。 在创建自定义用户流属性后，不能对此进行修改。 **dataType** 支持的值有：<br/><ul><li>`string` - 表示 identityUserFlowAttribute 的数据类型为字符串。 </li><li>`boolean` - 表示 identityUserFlowAttribute 的数据类型为Boolean。</li><li>`int64` - 表示 identityUserFlowAttribute 的数据类型为整数。</li></ul>|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```json
{
    "@odata.type": "#microsoft.graph.identityUserFlowAttribute",
    "id": "String (identifier)",
    "displayName": "String",
    "description": "String",
    "userFlowAttributeType": "String",
    "dataType": "String"
}
```
