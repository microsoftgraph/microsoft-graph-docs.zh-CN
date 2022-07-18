---
title: ediscoverySearch： purgeData
description: 使用清除数据方法在电子数据展示搜索中删除 Teams 消息。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 4a74360e6d714f34e23e6dc6a7ac2bbef641431d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446650"
---
# <a name="ediscoverysearch-purgedata"></a>ediscoverySearch： purgeData
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

永久删除 [电子数据展示搜索](../resources/security-ediscoverysearch.md)中包含的 Microsoft Teams 消息。

>**注意：** 此请求仅清除 Teams 数据。 它不会清除其他类型的数据，如邮箱项。

可以收集和清除以下类别的 Teams 内容：
- **Teams 1：1 聊天** - 两个人在 Teams 对话中共享的聊天消息、帖子和附件。 Teams 1：1 聊天也称为 *对话*。
- **Teams 群组聊天** - 三个或三个以上人员在 Teams 对话中共享的聊天消息、帖子和附件。 也称为 *1：N* 聊天或 *群组对话*。
- **Teams 频道** - 在标准 Teams 频道中共享的聊天消息、帖子、答复和附件。
- **专用频道** - 在专用 Teams 频道中共享的消息帖子、答复和附件。
- **共享频道** - 共享 Teams 频道中共享的消息帖子、答复和附件。

有关清除 Teams 消息的详细信息，请参阅：
- [电子数据展示解决方案系列：数据溢出方案 - 搜索和清除](/microsoft-365/compliance/data-spillage-scenariosearch-and-purge)
- [Advanced eDiscovery Microsoft Teams 中内容的工作流](/microsoft-365/compliance/teams-workflow-in-advanced-ediscovery) 


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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/purgeData
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。

如果清除数据操作成功启动，此操作将返回 `202 Accepted` 响应代码。 响应还将包含一个 `Location` 标头，其中包含为提交清除而创建的 [清除数据操作](../resources/security-ediscoverypurgedataoperation.md) 的位置。
若要检查清除数据操作的状态，请向位置 URL 发出 GET 请求。


## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverysearchthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/purgeData
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverysearchthispurgedata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverysearchthispurgedata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverysearchthispurgedata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/ediscoverysearchthispurgedata-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/ediscoverysearchthispurgedata-powershell-snippets.md)]
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
