---
title: 删除 customerPaymentJournals
description: 删除 Dynamics 365 Business Central 中的客户付款日志。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 0ddd675b617c679258b0f5de5363922b1e3e6d8d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791727"
---
# <a name="delete-customerpaymentjournals"></a>删除 customerPaymentJournals
从 Dynamics 365 Business Central 中删除客户付款日记对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型 |权限（从最低特权到最高特权）|
|:---------------|:------------------------------------------|
|委派（工作或学校帐户）|Financials.ReadWrite.All |
|委派（个人 Microsoft 帐户|不支持。|
|应用程序|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
```
DELETE /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头       |值                     |
|-------------|--------------------------|
|Authorization|Bearer {token}。必需。 |
|If-Match     |必需。 如果包含此请求标头，且提供的 eTag 与**customerPaymentJournals**上的当前标记不匹配，则不会更新**customerPaymentJournals** 。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 ```204 No Content``` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

**请求**

下面是一个请求示例。

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}
```

**响应** 

下面是一个响应示例。 

```json
HTTP/1.1 204 No Content
```

