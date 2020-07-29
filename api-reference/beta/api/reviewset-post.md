---
title: 创建 reviewSet
description: 创建电子数据展示检查集。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c16ef3c9e325e3c144cdec532cc81e6e31623138
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510018"
---
# <a name="create-reviewset"></a>创建 reviewSet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的[reviewSet](../resources/reviewset.md)对象。 请求正文包含审阅集的显示名称，该名称是唯一的可写属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | User.Read |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供[reviewSet](../resources/reviewset.md)的 JSON 表示形式。  下表列出了必需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| displayName  | string      | 评审集的名称。 |

## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[reviewSet](../resources/reviewset.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "post_reviewset"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
Content-type: application/json

{
  "displayName": "My Reviewset 3",
}
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
