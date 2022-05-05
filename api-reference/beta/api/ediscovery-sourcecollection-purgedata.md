---
title: sourceCollection： purgeData
description: 使用清除数据方法删除 sourceCollection 中敏感的Microsoft Teams消息。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: fa2bb5cb399d22302d167fd9fb120f13d43e3d43
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211425"
---
# <a name="sourcecollection-purgedata"></a>sourceCollection： purgeData

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

永久删除 [sourceCollection](../resources//ediscovery-sourcecollection.md) 中包含的Microsoft Teams消息。

>**注意：** 此请求仅清除Teams数据。 它不会清除其他类型的数据，如邮箱项。

可以收集和清除以下类别的Teams内容：
- **Teams 1：1 聊天** - 在两人Teams对话中共享的聊天消息、帖子和附件。 Teams 1：1 聊天也称为 *对话*。
- **Teams群聊天** - 在三个或更多人之间Teams对话中共享的聊天消息、帖子和附件。 也称为 *1：N* 聊天或 *群组对话*。
- **Teams频道** - 在标准Teams频道中共享的聊天消息、帖子、答复和附件。
- **专用频道** - 在专用Teams频道中共享的消息帖子、答复和附件。
- **共享频道** - 共享Teams通道中共享的消息帖子、答复和附件。

有关清除Teams消息的详细信息，请参阅：
- [电子数据展示解决方案系列：数据溢出方案 - 搜索和清除](/microsoft-365/compliance/data-spillage-scenariosearch-and-purge)
- [Advanced eDiscovery Microsoft Teams中内容的工作流](/microsoft-365/compliance/teams-workflow-in-advanced-ediscovery) 

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。

如果清除数据操作成功启动，此操作将返回 `202 Accepted` 响应代码。 响应还将包含一个 `Location` 标头，其中包含为提交清除而创建的 [清除数据操作](../resources/ediscovery-purgedataoperation.md) 的位置。
若要检查清除数据操作的状态，请向位置 URL 发出 GET 请求。 请求成功完成后， [状态](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) 将更改为 `succeeded`。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sourcecollectionthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sourcecollectionthispurgedata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sourcecollectionthispurgedata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sourcecollectionthispurgedata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sourcecollectionthispurgedata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/sourcecollectionthispurgedata-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/sourcecollectionthispurgedata-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
