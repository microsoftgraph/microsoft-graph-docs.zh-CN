---
title: 创建 allowedValue
description: 创建新的 allowedValue 对象。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a647525b112059c271a74cd691a2eaec4db6e724
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077693"
---
# <a name="create-allowedvalue"></a>创建 allowedValue
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [allowedValue](../resources/allowedvalue.md) 对象。

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
POST /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}/allowedValues
```


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [allowedValue](../resources/allowedvalue.md) 对象的 JSON 表示形式。

下表显示创建 [allowedValue](../resources/allowedvalue.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|预定义值的标识符。 可最多为 64 个字符，并且包含 Unicode 字符。 可以包含空格，但不允许使用某些特殊字符。 以后无法更改。 区分大小写。 必需。|
|isActive|布尔|指示预定义值是处于活动状态还是已停用。 如果设置为 `false` ，则此预定义值不能分配给任何其他受支持的目录对象。 必需。|



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [allowedValue](../resources/allowedvalue.md) 对象。

## <a name="examples"></a>示例

### <a name="example-add-a-predefined-value"></a>示例：添加预定义值

以下示例向自定义安全属性定义添加预定义值。

+ 属性集： `Engineering`
+ 属性： `Project`
+ 预定义值： `Alpine`

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_allowedvalue"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues
Content-Type: application/json

{
    "id":"Alpine",
    "isActive":"true"
}
```


#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.allowedValue"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions('Engineering_Project')/allowedValues/$entity",
    "id": "Alpine",
    "isActive": true
}
```
