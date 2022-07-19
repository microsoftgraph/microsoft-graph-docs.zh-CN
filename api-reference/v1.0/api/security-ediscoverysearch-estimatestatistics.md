---
title: ediscoverySearch： estimateStatistics
description: 运行电子数据展示搜索的估计值。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0809dbad83052bdd6a8de830df8cb522c61ba693
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839362"
---
# <a name="ediscoverysearch-estimatestatistics"></a>ediscoverySearch： estimateStatistics
命名空间：microsoft.graph.security

运行电子数据展示搜索中电子邮件和文档数的估计值。 若要详细了解电子数据展示中的搜索，请参阅电子数据 [展示 (高级) 中收集案例的数据 ](/microsoft-365/compliance/collecting-data-for-ediscovery)。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/estimateStatistics
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果估算成功启动，此操作将返回 `202 Accepted` 响应代码。
响应还将包含一个 `Location` 标头，其中包含为处理估算而创建的 [microsoft.graph.security.estimateStatisticsOperation](../resources/security-ediscoveryestimateoperation.md) 的位置。 通过向位置发出 GET 请求来检查估算操作的状态。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "ediscoverysearchthis.estimatestatistics"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/estimatestatistics
```


### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```