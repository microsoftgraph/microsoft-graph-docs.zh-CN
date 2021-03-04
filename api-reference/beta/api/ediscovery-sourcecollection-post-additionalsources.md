---
title: 创建 dataSource
description: 将其他数据源添加到源集合。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d2dca8b1b2ae6c6e1fc350f9b7185e16608427a7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445998"
---
# <a name="create-datasource"></a>创建 dataSource

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将其他数据源添加到源集合。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [dataSource](../resources/ediscovery-datasource.md) 对象的 JSON 表示形式。

下表显示创建 [dataSource](../resources/ediscovery-datasource.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|[sourceCollection](../resources/ediscovery-sourcecollection.md)案例的 ID。 只读。 继承自 [实体](../resources/entity.md)|
|displayName|String|[sourceCollection 的名称](../resources/ediscovery-sourcecollection.md)|
|createdDateTime|DateTimeOffset|创建 [sourceCollection 的](../resources/ediscovery-sourcecollection.md) 日期和时间。|
|createdBy|[identitySet](../resources/identityset.md)|创建 [sourceCollection 的用户](../resources/ediscovery-sourcecollection.md)。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
Content-Type: application/json
Content-length: 179

{
    "@odata.type": "#microsoft.graph.ediscovery.userSource",
    "email": "badguy@contoso.com"
}
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "id": "0fb67fc5-7fc5-0fb6-c57f-b60fc57fb60f",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```
