---
title: 更新 externalGroup
description: 更新 externalGroup 对象的属性。
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 52a818e5679d212a0afe1318c9125d1d8f88ffcd
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697506"
---
# <a name="update-externalgroup"></a>更新 externalGroup
命名空间：microsoft.graph.externalConnectors



更新 [externalGroup 对象](../resources/externalconnectors-externalgroup.md) 的属性。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持                               |
| 委派（个人 Microsoft 帐户） | 不支持                               |
| 应用程序                            | ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All             

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /connections/{connectionsId}/groups/{externalGroupId}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关属性的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为获得最佳性能，请勿包含未更改的属性。

| 属性    | 类型   | 说明                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| displayName | String | 外部组的友好名称。 可选。                                                                      |
| description | String | 外部组的说明。 可选。                                                                         |



## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_externalgroup"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/connections/{connectionsId}/groups/{externalGroupId}
Content-Type: application/json

{
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
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
