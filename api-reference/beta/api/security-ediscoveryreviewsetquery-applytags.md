---
title: ediscoveryReviewSetQuery： applyTags
description: 将标记应用到电子数据展示审阅集中的文件。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 94c9492804b1efc35247b5465d4b6b94b4b537f2
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945446"
---
# <a name="ediscoveryreviewsetquery-applytags"></a>ediscoveryReviewSetQuery： applyTags
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将标记应用到电子数据展示审阅集中的文件。 [了解详细信息。](https://docs.microsoft.com/microsoft-365/compliance/tagging-documents)

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries/{queryId}/applyTags
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
|tagsToAdd|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合|要从审阅集查询中的文件中删除的标记。|
|tagsToRemove|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合|用于删除在审阅集查询中添加文件的标记。|



## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetquerythis.applytags"
}
-->
``` http
POST https://graph.microsoft.com/beta/ediscoveryExportOperation/reviewSetQuery/applyTags
Content-Type: application/json

{
    "tagsToAdd": [
        {"id": "d3d99dc704a74801b792b3e1e722aa0d"}
    ]
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
HTTP/1.1 202 Accepted
```