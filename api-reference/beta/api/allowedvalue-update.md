---
title: 更新 allowedValue
description: 更新 allowedValue 对象的属性。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 119081faf43e32949314d2a601049b1a281ce443
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077479"
---
# <a name="update-allowedvalue"></a>更新 allowedValue
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [allowedValue 对象](../resources/allowedvalue.md) 的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CustomSecAttributeDefinition.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CustomSecAttributeDefinition.ReadWrite.All|

还必须为登录用户分配属性定义管理员 [目录角色](/azure/active-directory/roles/permissions-reference)。 默认情况下，全局管理员和其他管理员角色没有读取、定义或分配自定义安全属性的权限。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}/allowedValues/{allowedValueId}
```


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，*仅* 提供应更新的属性的值。未包含在请求正文中的现有属性将保留其以前的值或根据对其他属性值的更改重新计算。

下表指定可更新的属性。 

|属性|类型|Description|
|:---|:---|:---|
|isActive|布尔|指示预定义值是处于活动状态还是已停用。 如果设置为 `false` ，则此预定义值不能分配给任何其他受支持的目录对象。 可选。|



## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-deactivate-a-predefined-value"></a>示例：停用预定义值

以下示例停用自定义安全属性定义的预定义值。

+ 属性集： `Engineering`
+ 属性： `Project`
+ 预定义值： `Alpine`

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_allowedvalue"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues/Alpine
Content-Type: application/json
Content-length: 80

{
    "isActive": "false"
}
```


#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
