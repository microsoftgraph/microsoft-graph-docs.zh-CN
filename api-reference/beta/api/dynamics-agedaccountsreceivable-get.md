---
title: 获取 agedAccountsReceivable
description: 获取 Dynamics 365 Business Central 中的应收帐户应收对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
doc_type: apiPageType
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ec1eedd4055d575eb469336bb177114c1561daee
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046165"
---
# <a name="get-agedaccountsreceivable"></a>获取 agedAccountsReceivable

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 Dynamics 365 Business Central 的应收帐款报表对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型 |权限（从最低特权到最高特权）|
|:---------------|:------------------------------------------|
|委派（工作或学校帐户）|Financials.ReadWrite.All |
|委派 (个人 Microsoft 帐户|不支持。|
|应用程序|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
```http
GET /financials/companies/{id}/agedAccountsReceivable
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头|值|
|------|-----|
|Authorization  |Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **一个 agedAccountsReceivable** 对象。

## <a name="example"></a>示例

**请求**

下面是一个请求示例。

```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/agedAccountsReceivable?$filter=periodLengthFilter eq '3M'
```

**响应**

下面是一个响应示例。 

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

```json
{
  "customerId": "id-value",
  "customerNumber": "30000",
  "name": "Relecloud",
  "currencyCode": "USD",
  "balanceDue": 349615.45,
  "currentAmount": 0,
  "period1Amount": 349615.45,
  "period2Amount": 0,
  "period3Amount": 0,
  "agedAsOfDate": "2017-04-25",
  "periodLengthFilter": "3M"   
}
```


