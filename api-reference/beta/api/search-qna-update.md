---
title: 更新 qna
description: 更新 qna 对象的属性。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: da045a3ed91bdc6ad5441fe9a854d225c144208d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338403"
---
# <a name="update-qna"></a>更新 qna
命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [qna 对象](../resources/search-qna.md) 的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| SearchConfiguration.Read.All、SearchConfiguration.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| SearchConfiguration.Read.All、SearchConfiguration.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /search/qna/{qnaId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [qna](../resources/search-qna.md) 对象的 JSON 表示形式。 提供应更新的相关字段的值。 请求正文中未包含的现有属性将保留其以前的值或根据其他属性值的更改重新计算。 为了实现最佳性能，不得添加未变化的现有值。
>**注意：** 对集合属性的更新将更新整个集合。 对集合的任何更新（如关键字或类别）都将完全替换该集合。

|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|搜索结果中显示的问题。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|说明|String|搜索结果中显示的答案。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|webUrl|String|Qna URL 链接。 当用户在搜索结果中单击此 qna 时，他们将转到此 URL。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|availabilityStartDateTime|DateTimeOffset|qna 开始显示为搜索结果的时间戳。 设置为" `null` 始终可用"。|
|availabilityEndDateTime|DateTimeOffset|qna 停止显示为搜索结果的时间戳。 设置为" `null` 始终可用"。|
|languageTags|String collection|能够查看此问答的一个或多个国家/地区列表。|
|平台|microsoft.graph.devicePlatformType 集合|能够查看此问答的设备和操作系统列表。 可取值为：`unknown`、`android`、`androidForWork`、`ios`、`macOS`、`windowsPhone81`、`windowsPhone81AndLater`、`windows10AndLater`、`androidWorkProfile`、`androidASOP`。|
|targetedVariations|[microsoft.graph.search.answerVariant](../resources/search-answerVariant.md) 集合|qna 的变体，适用于不同的国家/地区或设备。 当你需要根据用户的设备、国家/地区或两者向用户显示不同的内容时，请使用 。 日期和组设置将应用于所有变体。|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|触发此 qna 显示在搜索结果中的关键字。|
|state|microsoft.graph.search.answerState|qna 的状态。 可能的值是：、`published``draft`、`excluded`或 `unknownFutureValue`。|
|groupIds|String collection|能够查看此 qna 的安全组列表。|



## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_qna"
}-->
``` http
PATCH https://graph.microsoft.com/beta/search/qna/{qnaId}
Content-Type: application/json

{
    "description": "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a weekend."
}
```


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}-->
``` http
HTTP/1.1 204 No Content
```

