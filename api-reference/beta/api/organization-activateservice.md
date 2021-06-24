---
title: organization： activateService
description: 为组织激活服务。
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6008b7f5a597af5ac65b349af22879b9db1255f4
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109160"
---
# <a name="organization-activateservice"></a>organization： activateService

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为组织激活服务。

## <a name="permissions"></a>权限
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

若要为组织激活服务，请求者需要具有以下权限的公司管理员角色。 

|权限类型|权限（从最低特权到最高特权）|
| :--- | :--- |
| 委派（工作或学校帐户） | Directory.ReadWrite.All|
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | Directory.ReadWrite.All|


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/activateService
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [activateService](../resources/activateService.md) 对象的 JSON 表示形式。
必须定义 **service 或 (** **servicePlanId** _和_ **skuId**) 此操作有效。

| 属性         | 类型         | 说明                           |
| ----------------- | ------------ | ------------------------------------- |
| service| String | 要激活的服务的名称。 |
| servicePlanId | Guid | 要激活的服务计划的计划标识符。 |
| skuId | Guid | 服务计划的 SKU 标识符。 |

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "organization_activateservice"
}
-->
``` http
POST https://graph.microsoft.com/beta/organization/{:organizationId}/activateService
Content-Type: application/json

{
    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900",
    "servicePlanId": "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
}
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```