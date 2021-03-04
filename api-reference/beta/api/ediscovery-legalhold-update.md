---
title: 更新 legalHold
description: 更新 legalHold 对象的属性。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6f44bc276bdc3ae5f23ce3243127a38d4e7a6063
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446036"
---
# <a name="update-legalhold"></a>更新 legalHold

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [legalHold 对象](../resources/ediscovery-legalhold.md) 的属性。

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
PATCH /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

|属性|类型|说明|
|:---|:---|:---|
|contentQuery|String|指定要位于指定位置的内容的 KQL 查询。 有关电子数据展示中的 KQL 详细信息，请参阅内容搜索和电子数据展示的关键字查询 [和搜索条件](/microsoft-365/compliance/keyword-queries-and-search-conditions)。 若要保留指定位置中所有内容，请保留 **contentQuery** 为空。 |
|说明|String| 法定保留说明。 |
|displayName|String| 法定显示名称的一部分。 |
|isEnabled|Boolean|指示是否启用保留并主动保留内容。 |

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_legalhold"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
Content-Type: application/json
Content-length: 295

{
  "description": "This is a description for a legalHold"
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 204 No Content
```
