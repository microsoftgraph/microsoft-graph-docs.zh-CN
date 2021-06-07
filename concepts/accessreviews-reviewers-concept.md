---
title: 使用 Microsoft Graph API 将审阅者分配给你的访问评审
description: 了解如何使用 Microsoft 网站中的访问评审 API Graph分配访问审阅者。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: bc6ada083b27a39fa26174c60f7637a02ec1cd8f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754928"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>使用 Microsoft Graph API 将审阅者分配给你的访问评审

Azure AD [访问评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 允许你以编程方式查看用户、服务主体或组对 Azure AD 资源的访问权限。

> [!NOTE]
> 访问[评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)目前仅适用于 Microsoft Graph beta 终结点。 请勿在生产应用中使用它，因为它可能会随时更改，恕不另行通知。

主要审阅者在访问评审 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)资源的 **reviewers** 属性中配置。  此外，可以使用 **fallbackReviewers** 属性指定回退审阅者。 创建自审阅网站时，不需要 (查看自己的访问权限) 。

## <a name="configure-reviewers"></a>配置审阅者

若要配置审阅者和回退审阅者，请设置 **accessReviewReviewerScope** 的 **query、queryRoot** 和 **queryType** 属性的值。  有关这些属性的说明，请参阅 [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true) 资源类型。

### <a name="example-1-a-specific-user-as-the-reviewer"></a>示例 1：作为审阅者的特定用户

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-2-members-of-a-group-as-reviewers"></a>示例 2：作为审阅者的组的成员

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-group-owners-as-reviewers"></a>示例 3：作为审阅者的组所有者
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

### <a name="example-4-people-managers-as-reviewers"></a>示例 4：作为审阅者的人经理

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```
由于 `./manager` 是相对查询，因此请用值 指定 **queryRoot** 属性 `decisions` 。

## <a name="see-also"></a>另请参阅

+ [配置访问评审定义的范围](/graph/accessreviews-scope-concept)
