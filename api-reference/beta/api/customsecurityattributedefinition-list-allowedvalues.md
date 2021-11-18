---
title: 列出 allowedValues
description: 获取 allowedValue 对象及其属性的列表。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c326845bb8a6b493629b8d6a2dd566bd3f349f4c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077697"
---
# <a name="list-allowedvalues"></a>列出 allowedValues
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [allowedValue 对象](../resources/allowedvalue.md) 及其属性的列表。

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
GET /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}/allowedValues
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

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [allowedValue](../resources/allowedvalue.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-get-all-predefined-values"></a>示例：获取所有预定义值

以下示例获取自定义安全属性定义的所有预定义值。

+ 属性集： `Engineering`
+ 属性： `Project`

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_allowedvalue"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues
```


#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.allowedValue)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions('Engineering_Project')/allowedValues",
    "value": [
        {
            "id": "Cascade",
            "isActive": true
        },
        {
            "id": "Baker",
            "isActive": true
        },
        {
            "id": "Alpine",
            "isActive": true
        }
    ]
}
```
