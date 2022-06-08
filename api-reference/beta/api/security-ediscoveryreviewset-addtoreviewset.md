---
title: ediscoveryReviewSet：addToReviewSet
description: 开始将集合从 Microsoft 365 服务添加到审阅集的过程。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8ae8a25bb90e647c4bd4795febf321a2a7208421
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945448"
---
# <a name="ediscoveryreviewset-addtoreviewset"></a>ediscoveryReviewSet：addToReviewSet
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

开始将集合从 Microsoft 365 服务添加到审阅集的过程。 创建操作后，可以通过从响应标头中检索 `Location` 参数来获取操作的状态。 该位置提供一个 URL，该 URL 将返回 [“添加到审阅”集操作](../resources/security-ediscoveryaddtoreviewsetoperation.md)。


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
POST /ediscoveryExportOperation/reviewSet/addToReviewSet
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|要添加到审阅集的电子数据展示搜索的 ID。|
|additionalDataOptions|additionalDataOptions|用于将项目添加到 reviewSet 的选项。|

### <a name="additionaldataoptions-values"></a>additionalDataOptions 值
|名称|说明|
|:---|:---|
|allVersions|包括与源集合查询匹配的 sharepoint 文档的所有版本。 注意：SharePoint 版本可以显著增加项目量 |
|linkedFiles|通过将链接附加到该文件，包括在 outlook、teams 或 yammer 消息中共享的链接文件。|

## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetthis.addtoreviewset"
}
-->
``` http
POST https://graph.microsoft.com/beta/ediscoveryExportOperation/reviewSet/addToReviewSet
Content-Type: application/json

{
    "search": {
        "id": "7c165312-d8db-48b5-9129-1af50932df53"
    },
    "additionalDataOptions": "linkedFiles"
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