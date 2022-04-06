---
title: sourceCollection： purgeData
description: 使用清除数据方法可删除 sourceCollection 中Microsoft Teams错误放置的邮件。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a7a2e7ae0138f57739184325b2615d90d74d5abb
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608410"
---
# <a name="sourcecollection-purgedata"></a>sourceCollection： purgeData

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

永久删除Microsoft Teams[包含在 sourceCollection 中的邮件](../resources//ediscovery-sourcecollection.md)。

>**注意：** 此请求仅Teams数据。 它不会清除其他类型的数据，如邮箱项目。

可以收集和清除以下类别的Teams内容：
- **Teams一对一** 聊天 - 在两个人之间的对话中共享的聊天Teams帖子和附件。 Teams一对一聊天也称为 *对话*。
- **Teams群** 聊 - 在三个或多个人员之间的群组对话中Teams聊天消息、帖子和附件。 也称为 *1：N* 聊天或 *群组对话*。
- **Teams频道** - 在标准频道中共享的聊天消息、帖子、回复和Teams附件。
- **私人频道** - 私人频道中共享的消息帖子、回复和Teams附件。
- **共享频道** - 共享频道中共享的消息帖子、回复和Teams附件。

有关清除邮件Teams，请参阅：
- [电子数据展示解决方案系列：数据泄漏方案 - 搜索和清除](/microsoft-365/compliance/data-spillage-scenariosearch-and-purge)
- [Advanced eDiscovery工作流中的内容Microsoft Teams](/microsoft-365/compliance/teams-workflow-in-advanced-ediscovery) 

## <a name="permissions"></a>Permissions

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

如果清除数据操作成功启动，此操作将返回 响应 `202 Accepted` 代码。 响应还将包含标头`Location`，其中包含为提交清除而创建的"清除数据[](../resources/ediscovery-purgedataoperation.md)"操作的位置。
若要检查清除数据操作的状态，请对位置 URL 提出 GET 请求。 当请求成功完成时， [状态](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) 将更改为 `succeeded`。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "sourcecollectionthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
