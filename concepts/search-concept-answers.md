---
title: '为组织中用户设置管理搜索答案 (预览) '
description: Microsoft 搜索使管理员能够将搜索词与特定于其组织的含义或网页关联，并将这些关联作为搜索答案。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 542f1c3dc3d280ba72c3c64d032c19594c6bc29c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337891"
---
# <a name="set-up-administrative-search-answers-for-users-in-an-organization-preview"></a>为组织中用户设置管理搜索答案 (预览) 

Microsoft 搜索使管理员能够将搜索词与特定于其组织的含义或网页关联，并将这些关联作为搜索答案。 例如，组织的用户可能会遇到一个不熟悉的缩写词，该缩写词代表内部项目名称或与工作组网页关联的工作组名称。 管理员可以在"搜索和[](/microsoftsearch/manage-acronyms)智能["](/microsoftsearch/manage-bookmarks)下的Microsoft 365 管理中心设置首字母缩写词、书签& [](https://admin.microsoft.com/)[QnA](/microsoftsearch/manage-qas)。 这使用户能够使用搜索来导航和熟悉他们的工作。

管理员还可使用 Microsoft Graph以编程方式管理组织中管理搜索答案。 当由可用搜索应答Microsoft 搜索类型（首字母缩写、书签和 [QnA](/graph/api/resources/search-qna) 资源）中定义的缩写词或关键字触发时，这些答案将显示在[](/graph/api/resources/search-acronym)结果中。 [](/graph/api/resources/search-bookmark)

当由定义的缩写词或关键字触发时，这些搜索答案将显示在您组织的搜索结果页面的顶部。

## <a name="example-create-a-new-acronym"></a>示例：创建新的缩写词

以下请求创建一个新的缩写词，当用户搜索搜索结果页面时，该缩写词会显示在搜索结果页面上。

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

## <a name="example-create-a-new-bookmark"></a>示例：创建新书签

以下请求创建一个新书签，当用户搜索其至少一个关键字时，该书签会显示在搜索结果页面上。

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
- 熟悉搜索 API 方案和功能：Microsoft 搜索 [API 概述](/graph/search-concept-overview)。
- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 中浏览搜索 API。
- [管理管理搜索答案](search-concept-answers.md)。
