---
title: identityUserFlowAttribute 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的用户流属性。
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: ea7448bcb4e805042870b7648b91d47a478948f3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067344"
---
# <a name="identityuserflowattribute-resource-type"></a>identityUserFlowAttribute 资源类型

命名空间：microsoft.graph

表示 Azure Active Directory （Azure AD） 租户中的用户流属性。

在 Azure AD 租户中配置用户流属性可让你在注册期间收集用户相关信息。 可以选择收集一组内置属性。 例如，给定姓名、省/市/县和邮政编码。 还可以配置自定义用户流属性，以便收集未内置到目录中的用户的信息。 自定义用户流属性是对[Azure Active Directory 架构扩展](/azure/active-directory/develop/active-directory-schema-extensions)的抽象。

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
|userFlowAttributeType|identityUserFlowAttributeType|用户流属性的类型。 这是一个自动设置的只读属性。 根据属性的类型，此属性的值将为 `builtIn`、 `custom`或 `required`。|
|DataType|identityUserFlowAttributeDataType|用户流属性的数据类型。 在创建自定义用户流属性后，不能对此进行修改。 数据类型 **支持** 为： `string` 、 `boolean` 、 `int64` 、 `stringCollection` 、 `dateTime`。|

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
