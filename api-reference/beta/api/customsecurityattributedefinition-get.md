---
title: 获取 customSecurityAttributeDefinition
description: 读取 customSecurityAttributeDefinition 对象的属性和关系。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5320e7a1dc78814a77fe6d62dbaf2b3d25c72c62
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077701"
---
# <a name="get-customsecurityattributedefinition"></a>获取 customSecurityAttributeDefinition
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CustomSecAttributeAssignment.ReadWrite.All、CustomSecAttributeDefinition.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CustomSecAttributeAssignment.ReadWrite.All、CustomSecAttributeDefinition.ReadWrite.All|

还必须为登录用户分配以下目录角色之 [一](/azure/active-directory/roles/permissions-reference)：

+ 属性定义读取器
+ 属性分配管理员
+ 属性定义管理员

默认情况下，全局管理员和其他管理员角色没有读取、定义或分配自定义安全属性的权限。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) 对象。

## <a name="examples"></a>示例

### <a name="example-get-a-custom-security-attribute"></a>示例：获取自定义安全属性

以下示例获取单个自定义安全属性定义。

+ 属性集： `Engineering`
+ 属性： `ProjectDate`

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_customsecurityattributedefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_ProjectDate
```


#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->
``` http
HTTP/1.1 200 OK
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
