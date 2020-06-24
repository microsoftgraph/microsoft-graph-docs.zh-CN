---
title: 创建 connectorGroup
description: 创建 connectorGroup 对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ddc1aebfeb64e4dd596f94dd8a91f3718a29fb7
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863262"
---
# <a name="create-connectorgroup"></a>创建 connectorGroup

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建[connectorGroup](../resources/connectorgroup.md)对象。

## <a name="permissions"></a>权限
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a>可选的请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | 负载. 必需。|
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供[connectorGroup](../resources/connectorgroup.md)对象的 JSON 表示形式。
下表列出了可用于**connectorGroup**的属性。 **Name**属性是必需属性。

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|connectorGroupType|字符串| 指示混合代理的类型。 此属性由系统预设。|
|id|string| 此 connectorGroup 的唯一标识符。 只读。 |
|isDefault|boolean| 指示 connectorGroup 是否为默认值。 只有一个连接器组可以是默认的 connectorGroup，这是由系统预设的。 |
|name|string| 与 connectorGroup 关联的名称。 |
|范围|字符串| 向其分配 connectorGroup 的区域并将为其优化流量。 仅当**未**向 connectorGroup 分配连接器或应用程序时，才能设置此区域。 可用区域包括：北美、欧洲、澳大利亚、亚洲和印度。 可取值为：`nam`、`eur`、`aus`、`asia`、`ind`。|

## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[connectorGroup](../resources/connectorgroup.md)对象。
## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "Connector Group Demo"

}
```
### <a name="response"></a>响应
下面展示了示例响应。 

>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "Connector Group Demo",
  "connectorGroupType": "applicationProxy",
  "isDefault": true,
  "region": "nam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
