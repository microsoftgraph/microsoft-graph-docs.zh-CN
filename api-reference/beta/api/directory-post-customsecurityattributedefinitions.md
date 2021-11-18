---
title: 创建 customSecurityAttributeDefinition
description: 创建新的 customSecurityAttributeDefinition 对象。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: af0ff215715abf54f57c31a6920bf7953fcd726d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077471"
---
# <a name="create-customsecurityattributedefinition"></a>创建 customSecurityAttributeDefinition
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CustomSecAttributeDefinition.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CustomSecAttributeDefinition.ReadWrite.All|

还必须为登录用户分配属性定义管理员 [目录角色] (/azure/active-directory/roles/permissions-reference。 默认情况下，全局管理员和其他管理员角色没有读取、定义或分配自定义安全属性的权限。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directory/customSecurityAttributeDefinitions
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 对象的 JSON 表示形式。

下表显示可在创建自定义 [SecurityAttributeDefinition 时配置的属性](../resources/customsecurityattributedefinition.md)。

|属性|类型|Description|
|:---|:---|:---|
|attributeSet|String|属性集的名称。 不区分大小写。 必需。|
|description|String|自定义安全属性的说明。 可最多为 128 个字符，并且包含 Unicode 字符。 不能包含空格或特殊字符。 稍后可更改。 可选。|
|isCollection|布尔|指示是否可以将多个值分配给自定义安全属性。 以后无法更改。 如果 `type` 设置为 Boolean， `isCollection` 则不能设置为 true。 必需。|
|isSearchable|布尔|指示是否将为自定义安全属性值编制索引，以在分配了属性值的对象上搜索。 以后无法更改。 必需。|
|name|String|自定义安全属性的名称。 在属性集内必须是唯一的。 可最多为 32 个字符，并且包含 Unicode 字符。 不能包含空格或特殊字符。 以后无法更改。 不区分大小写。 必需。|
|status|String|指定自定义安全属性是处于活动状态还是已停用。 可接受的值为 和 `Available` `Deprecated` 。 稍后可更改。 此为必需属性。|
|type|String|自定义安全属性值的数据类型。 支持的类型包括 `Boolean` 、 `Integer` 和 `String` 。 以后无法更改。 必需。|
|usePreDefinedValuesOnly|布尔|指示是否只能将预定义值分配给自定义安全属性。 如果设置为 false，则允许自由格式的值。 稍后可以从 true 更改为 false，但无法从 false 更改为 true。 如果 `type` 设置为 Boolean， `usePreDefinedValuesOnly` 则不能设置为 true。 必需。|

`id`该属性是自动生成的，不能设置。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-add-a-custom-security-attribute"></a>示例 1：添加自定义安全属性

以下示例添加一个新的自定义安全属性定义，该定义是 String 类型的单个自由格式值。

+ 属性集： `Engineering`
+ 属性： `ProjectDate`

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_customsecurityattributedefinition"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions
Content-Type: application/json

{
    "attributeSet":"Engineering",
    "description":"Target completion date",
    "isCollection":false,
    "isSearchable":true,
    "name":"ProjectDate",
    "status":"Available",
    "type":"String",
    "usePreDefinedValuesOnly": false
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions/$entity",
    "attributeSet": "Engineering",
    "description": "Target completion date",
    "id": "Engineering_ProjectDate",
    "isCollection": false,
    "isSearchable": true,
    "name": "ProjectDate",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": false
}
```

### <a name="example-2-add-a-custom-security-attribute-that-supports-multiple-predefined-values"></a>示例 2：添加支持多个预定义值的自定义安全属性

以下示例添加一个新的自定义安全属性定义，该定义支持预定义的 String 类型的多个值。

+ 属性集： `Engineering`
+ 属性： `Project`

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_customsecurityattributedefinition_v2"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions
Content-Type: application/json
Content-length: 310

{
    "attributeSet":"Engineering",
    "description":"Active projects for user",
    "isCollection":true,
    "isSearchable":true,
    "name":"Project",
    "status":"Available",
    "type":"String",
    "usePreDefinedValuesOnly": true
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions/$entity",
    "attributeSet": "Engineering",
    "description": "Active projects for user",
    "id": "Engineering_Project",
    "isCollection": true,
    "isSearchable": true,
    "name": "Project",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": true
}
```
