---
title: 更新 unitsOfMeasure
description: 更新 Dynamics 365 Business Central 中的度量单位对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2dbaab40ef021024535591a33c76af56f8fe0642
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044828"
---
# <a name="update-unitsofmeasure"></a>更新 unitsOfMeasure

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 Dynamics 365 Business Central 的度量对象单位的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型 |权限（从最低特权到最高特权）|
|:---------------|:------------------------------------------|
|委派（工作或学校帐户）|Financials.ReadWrite.All |
|委派 (个人 Microsoft 帐户|不支持。|
|应用程序|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

```
PATCH /financials/companies/{id}/unitsOfMeasure/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头|值|
|------|-----|
|Authorization |Bearer。 必需。|
|Content-Type  |application/json|
|If-Match      |必需。 如果包含此请求标头且提供的 eTag 与 **unitsOfMeasure** 上的当前标记不匹配，将不会更新 **unitsOfMeasure。** |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` **unitsOfMeasure** 对象。

## <a name="example"></a>示例

**请求**

下面是一个请求示例。
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure/{id}
Content-type: application/json

{
  "displayName": "One Piece"
}
```

**响应**

下面是一个响应示例。 

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "One Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```



