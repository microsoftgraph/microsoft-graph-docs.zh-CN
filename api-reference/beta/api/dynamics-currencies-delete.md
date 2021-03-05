---
title: 删除货币
description: 删除 Dynamics 365 Business Central 中的货币对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b9f6c729dc97d523952454978afc056c05c354c5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473152"
---
# <a name="delete-currencies"></a>删除货币

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从 Dynamics 365 Business Central 中删除货币对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型 |权限（从最低特权到最高特权）|
|:---------------|:------------------------------------------|
|委派（工作或学校帐户）|Financials.ReadWrite.All |
|委派 (个人 Microsoft 帐户|不支持。|
|应用程序|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
```
DELETE /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头

|标头|值|
|------|-----|
|Authorization  |Bearer {token}。必需。 |
|If-Match       |必填。 如果包含此请求标头且提供的 eTag 与货币上的当前标记不匹配，**则货币** 不会
 更新。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回 ```204 No Content``` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

**请求**

下面是一个请求示例。

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

**响应** 

下面是一个响应示例。 

```http
HTTP/1.1 204 No Content
```


