---
title: 使用 Microsoft 图形 API 将审阅者分配给你的访问图形 API
description: 了解如何使用 Microsoft 网站中的访问评审 API Graph分配访问审阅者。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 099419f3c1998b94f1c57d983b8d25af0b653faf
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510651"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>使用 Microsoft 图形 API 将审阅者分配给你的访问图形 API

访问Azure AD [API](/graph/api/resources/accessreviewsv2-overview) 允许你以编程方式查看用户、服务主体或组对访问你的Azure AD的访问权限。

主要审阅者在访问评审 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) 资源的 **reviewers** 属性中配置。  此外，可以使用 **fallbackReviewers** 属性指定回退审阅者。 创建自审阅网站时，不需要 (查看自己的访问权限) 。

## <a name="configure-reviewers"></a>配置审阅者

若要配置审阅者和回退审阅者，请设置 **accessReviewReviewerScope** 的 **query**、**queryRoot** 和 **queryType** 属性的值。 有关这些属性的说明，请参阅 [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope) 资源类型。

### <a name="example-1-a-self-review"></a>示例 1：自我审阅

```http
"reviewers": []
```

若要配置自审阅，请不要指定 **reviewers** 属性，或为该属性提供空对象。

如果相应的访问评审 **范围面向** B2B 直接连接用户和具有共享频道的团队，将指派团队所有者查看 B2B 直接连接用户的访问权限。

### <a name="example-2-a-specific-user-as-the-reviewer"></a>示例 2：作为审阅者的特定用户

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-members-of-a-group-as-reviewers"></a>示例 3：作为审阅者的组的成员

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-4-group-owners-as-reviewers"></a>示例 4：作为审阅者的组所有者
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

若要仅将特定国家/地区中的组所有者分配为审阅者，

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

### <a name="example-5-people-managers-as-reviewers"></a>示例 5：作为审阅者的人经理

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```

由于 `./manager` 是相对查询，因此请用值 指定 **queryRoot** 属性 `decisions`。

如果相应的访问评审 **范围面向** B2B 直接连接用户和具有共享频道的团队，将指派团队所有者查看 B2B 直接连接用户的访问权限。

### <a name="example-6-application-owners-as-reviewers"></a>示例 6：作为审阅者的应用程序所有者

```http
"reviewers": [
    {
        "query": "/servicePrincipals/{id}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="next-steps"></a>后续步骤

+ [配置访问评审定义的范围](/graph/accessreviews-scope-concept)
+ [试用教程，](/graph/accessreviews-overview)了解如何使用访问评审 API 查看对Azure AD的访问权限
+ [创建访问评审](/azure/active-directory/governance/create-access-review)