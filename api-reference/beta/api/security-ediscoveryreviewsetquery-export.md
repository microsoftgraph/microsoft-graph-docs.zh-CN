---
title: ediscoveryReviewSetQuery：导出
description: 从 reviewSet 查询启动导出。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: aefa42a52c9b9619db9c3fd4c7a499d8961db39f
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945489"
---
# <a name="ediscoveryreviewsetquery-export"></a>ediscoveryReviewSetQuery：导出
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从 **reviewSet** 查询启动导出。  有关详细信息，请参阅 [高级电子数据展示中审阅集的](/microsoft-365/compliance/export-documents-from-review-set)导出文档。


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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries/{queryId}/export
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

如果成功，此操作返回 `202 Accepted` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetquerythis.export"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries/fcb86cd1-50e0-427c-840e-ba6f087364e5/export
Content-Type: application/json

{
    "outputName": "Export reviewset query via API",
    "description": "Export for the Contoso investigation 2",
    "exportOptions": "originalFiles,fileInfo,tags",
    "exportStructure": "directory"
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
