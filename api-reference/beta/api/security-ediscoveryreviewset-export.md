---
title: ediscoveryReviewSet：导出
description: 从 reviewSet 启动导出。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d009c516409b15b5d10a9bb8befb0d7e5b66bac5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092382"
---
# <a name="ediscoveryreviewset-export"></a>ediscoveryReviewSet：导出
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从 **reviewSet** 启动导出。  有关详细信息，请参阅[Advanced eDiscovery中审阅集的导出文档](/microsoft-365/compliance/export-documents-from-review-set)。


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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/export
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
|outputName|String| 导出的名称。 必需。 |
|description|String| 导出说明 |
|azureBlobContainer|String| 导出到自己的 Azure 存储帐户时，这是容器 URL。 |
|azureBlobToken|String| 导出到自己的 Azure 存储帐户时，容器 URL 的 SAS 令牌。 |
|exportOptions|String|指定控制导出格式的选项。 可取值为：`originalFiles`、`text`、`pdfReplacement`、`fileInfo`、`tags`。|
|exportStructure|String| 用于控制导出的文件结构和打包的选项。 可取值为：`none`、`directory`、`pst`。|
## <a name="response"></a>响应

如果导出已成功启动，此操作将返回 `202 Accepted` 响应代码。 响应还将包含一个 `Location` 标头，其中包含为处理导出而创建的 [导出操作](../resources/security-ediscoveryexportoperation.md) 的位置。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetthis.export"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/export
Content-Type: application/json

{
    "outputName": "Export via API",
    "description": "Export for the Contoso investigation",
    "exportOptions": "originalFiles,fileInfo,tags",
    "exportStructure": "directory"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoveryreviewsetthisexport-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoveryreviewsetthisexport-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoveryreviewsetthisexport-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/ediscoveryreviewsetthisexport-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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

