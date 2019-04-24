---
title: 删除 paymentTerms
description: 删除 Dynamics 365 Business Central 中的付款期限对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2ab608cc7e8f0e6ea17ea9911746fea52fc66a7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458689"
---
# <a name="delete-paymentterms"></a>删除 paymentTerms
从 Dynamics 365 Business Central 中删除付款条款对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型 |权限（从最低特权到最高特权）|
|:---------------|:------------------------------------------|
|委派（工作或学校帐户）|Financials.ReadWrite.All |
|委派 (个人 Microsoft 帐户|不支持。|
|应用程序|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
```
DELETE /financials/companies('{id}')/paymentTerms('{id}')
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头

|标头         |值                     |
|---------------|--------------------------|
|Authorization  |Bearer {token}。必需。 |
|If-Match       |必需。 如果包含此请求标头, 且提供的 eTag 与**paymentTerms**上的当前标记不匹配, 则不会更新**paymentTerms** 。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回 ```204 No Content``` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

**请求**

下面是一个请求示例。

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/paymentTerms('{id}')
```

**响应** 

下面是一个响应示例。 

```json
HTTP/1.1 204 No Content
```
