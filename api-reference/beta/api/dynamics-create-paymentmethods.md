---
title: 创建 paymentMethods
description: 在 Dynamics 365 Business Central 中创建付款方法对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 106c282c757362b7201afc3fd64d3b5a44920070
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791923"
---
# <a name="create-paymentmethods"></a>创建 paymentMethods
在 DDynamics 365 Business Central 中创建付款方法对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型 |权限（从最低特权到最高特权）|
|:---------------|:------------------------------------------|
|委派（工作或学校帐户）|Financials.ReadWrite.All |
|委派（个人 Microsoft 帐户|不支持。|
|应用程序|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
```
POST /financials/companies/{id}/paymentMethods
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头         |值                        |
|---------------|-----------------------------|
|Authorization  |Bearer {token}。必需。    |
|Content-Type   |application/json             |

## <a name="request-body"></a>请求正文
在请求正文中，提供**paymentMethods**对象的 JSON 表示形式。

## <a name="response"></a>响应
如果成功，此方法在```201 Created```响应正文中返回响应代码和**paymentMethods**对象。

## <a name="example"></a>示例

**请求**

下面是一个请求示例。

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
}
```

**响应**

下面是一个响应示例。 

> **注意**：为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都将通过实际调用返回。

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}

```

