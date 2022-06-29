---
title: '为组织中的用户设置管理搜索答案 (预览) '
description: Microsoft 搜索允许管理员将搜索词与特定于其组织的含义或网页相关联，并将其作为搜索答案包含在内。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: ffc0e35f351a0841b8905c73454d1461f7fb7013
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446103"
---
# <a name="set-up-administrative-search-answers-for-users-in-an-organization-preview"></a>为组织中的用户设置管理搜索答案 (预览) 

Microsoft 搜索允许管理员将搜索词与特定于其组织的含义或网页相关联，并将这些关联作为搜索答案包括在内。 例如，组织中的用户可能会遇到一个不熟悉的首字母缩略词，该首字母缩略词表示内部项目名称或与团队网页关联的团队名称。 管理员可以在搜索&**智能** 下，在 [Microsoft 365 管理中心](https://admin.microsoft.com/)中设置 [首字母缩写词](/microsoftsearch/manage-acronyms)、[书签](/microsoftsearch/manage-bookmarks)或 [QnA](/microsoftsearch/manage-qas)。 这使用户能够使用搜索导航并熟悉其工作。

管理员还可以使用 Microsoft Graph 中的 Microsoft 搜索 API 以 [编程方式管理组织中的管理搜索答案](/graph/api/resources/search-api-answers-overview) 。 当由可用搜索答案资源类型中定义的首字母缩略词或关键字触发时，这些答案将显示在 Microsoft 搜索结果中： [首字母缩略词](/graph/api/resources/search-acronym)、 [书签](/graph/api/resources/search-bookmark)和 [QnA](/graph/api/resources/search-qna) 资源。

当由定义的首字母缩略词或关键字触发时，这些搜索答案将显示在组织中搜索结果页面的顶部。

## <a name="example-1-create-a-new-acronym"></a>示例 1：创建新的首字母缩略词

以下请求将创建一个新的首字母缩略词，该首字母缩略词将在用户搜索时显示在搜索结果页上。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_acronym_from_acronyms"
}-->
```http
POST https://graph.microsoft.com/beta/search/acronyms
Content-Type: application/json

{
  "displayName": "GDPR",
  "standsFor": "General Data Protection Regulation",
  "description": "A European Union (EU) regulation on data protection and privacy in the EU and the European Economic Area (EEA) that enhances individuals' control and rights over their personal data, simplifies the regulatory environment for international business, and addresses the transfer of personal data outside the EU and EEA areas.",
  "webUrl": "http://contoso.com/GDPR",
  "state": "published"
}
```

### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.acronym"
}-->
```http
HTTP/1.1 200 Ok
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

## <a name="example-2-create-a-new-bookmark"></a>示例 2：创建新的书签

以下请求创建一个新的书签，当用户搜索其至少一个关键字时，该书签将显示在搜索结果页上。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_bookmark_from_bookmarks"
}-->
```http
POST https://graph.microsoft.com/beta/search/bookmarks
Content-Type: application/json

{
  "displayName": "Contoso Install Site",
  "webUrl": "http://www.contoso.com/",
  "description": "Try or buy Contoso for Home or Business and view product information",
  "keywords":  {
    "keywords": ["Contoso", "install"],
    "reservedKeywords": ["Contoso"],
    "matchSimilarKeywords": true
  },
  "state": "published"
}
```

### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.bookmark"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

## <a name="next-steps"></a>后续步骤

- 熟悉搜索 API 方案和功能： [Microsoft 搜索 API 概述](/graph/search-concept-overview)。
- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 中浏览搜索 API。
- [使用 Microsoft 搜索 API 管理管理答案](/graph/api/resources/search-api-answers-overview)。
