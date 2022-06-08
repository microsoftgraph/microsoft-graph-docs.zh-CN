---
title: 更新 ediscoverySearch
description: 更新 ediscoverySearch 对象的属性。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 981e9098695789fee2bf60ff8466d2b7c5a411c6
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945377"
---
# <a name="update-ediscoverysearch"></a>更新 ediscoverySearch
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [ediscoverySearch 对象的](../resources/security-ediscoverysearch.md) 属性。

## <a name="permissions"></a>权限
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
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|contentQuery|字符串|KQL (关键字查询语言) 查询中的查询字符串。 有关详细信息，请参阅 [内容搜索和电子数据展示的关键字查询和搜索条件](/microsoft-365/compliance/keyword-queries-and-search-conditions)。  可以使用与值配对的字段来优化搜索;例如， `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016`.|
|dataSourceScopes|dataSourceScopes|指定后，集合将跨整个工作负荷的服务。 可能的值为：，`none``allTenantMailboxes`，`allTenantSites`，`allCaseCustodians`，`allCaseNoncustodialDataSources`。 **注意：** 创建源集合时，需要一个保管人或指定 dataSourceScope。|
|description|String|**电子数据展示搜索** 的说明。|
|displayName|String|**电子数据展示搜索** 的显示名称。|


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和更新 [的 ediscoverySearch](../resources/security-ediscoverysearch.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "update_ediscoverysearch"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}
Content-Type: application/json

{
    "displayName": "Teams search"
}
```


### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```