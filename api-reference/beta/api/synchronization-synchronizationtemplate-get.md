---
title: 获取 synchronizationTemplate
description: 按其标识符检索同步模板。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e0f5ff93cc87bd5c4cca2ada9891ba8ce4d02ac4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471158"
---
# <a name="get-synchronizationtemplate"></a>获取 synchronizationTemplate

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

按其标识符检索同步模板。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     |Directory.ReadWrite.All  |
|委派（个人 Microsoft 帐户） |不支持。|
|应用程序                            |不支持。| 

### <a name="http-request"></a>HTTP 请求

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a>请求标头

| 名称           | 类型    | 说明|
|:---------------|:--------|:-----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。

### <a name="example"></a>示例

##### <a name="request"></a>请求
请求示例如下所示。

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a>响应
响应示例如下所示。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性将在实际调用中返回。

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
