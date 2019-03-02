---
title: 获取 journalLines
description: 获取 Dynamics 365 Business Central 中的日记行对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 361731a346d1a7e649d92629d41d9aa83a4cf5d2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366660"
---
# <a name="get-journallines"></a>获取 journalLines
检索 Dynamics 365 Business Central 的日记行对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型 |权限（从最低特权到最高特权）|
|:---------------|:------------------------------------------|
|委派（工作或学校帐户）|Financials.ReadWrite.All |
|委派 (个人 Microsoft 帐户|不支持。|
|应用程序|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

```
GET /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头       |值                     |
|-------------|--------------------------|
|Authorization|Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功, 此方法在响应`200 OK`正文中返回响应代码和**journalLines**对象。

## <a name="example"></a>示例

**请求**

下面是一个请求示例。
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

**响应**

下面是一个响应示例。 

> **注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。 所有属性都将通过实际调用返回。

```json
{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

