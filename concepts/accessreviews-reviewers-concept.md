---
title: 使用 Microsoft 图形 API 将审阅者分配到访问评审
description: 使用 Microsoft Graph 中的访问评审 API 分配访问评审者，例如特定用户、组的成员或所有者、人员管理器或应用所有者。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: ce0e806920b2bb925cc16b7d31aa57156388935a
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698343"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>使用 Microsoft 图形 API 将审阅者分配到访问评审

使用 Azure AD [访问评审 API](/graph/api/resources/accessreviewsv2-overview) ，可以以编程方式查看用户、服务主体或组对 Azure AD 资源的访问权限。

主要审阅者配置在访问评审 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) 资源的 **审阅者** 属性中。  此外，还可以使用 **fallbackReviewers** 属性指定回退审阅者。 创建自审 (时不需要这些属性，用户会在其中查看自己的访问权限) 。

若要配置审阅者和回退审阅者，请设置 **accessReviewReviewerScope** 的 **查询**、**queryRoot** 和 **queryType** 属性的值。 有关这些属性的说明，请参阅 [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope) 资源类型。

## <a name="example-1-a-self-review"></a>示例 1：自我审阅

```http
"reviewers": []
```

若要配置自审阅，请勿指定 **审阅者** 属性，或向该属性提供空对象。

如果相应的访问评审 **范围** 面向具有共享通道的 B2B 直接连接用户和团队，则将分配团队所有者来评审 B2B 直接连接用户的访问权限。

## <a name="example-2-a-specific-user-as-the-reviewer"></a>示例 2：特定用户作为审阅者

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="example-3-members-of-a-group-as-reviewers"></a>示例 3：组成员作为审阅者

```http
"reviewers": [
    {
        "query": "/groups/{group id}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="example-4-group-owners-as-reviewers"></a>示例 4：组所有者作为审阅者
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

若要仅将特定国家/地区的组所有者分配为审阅者，请执行以下操作：

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

## <a name="example-5-people-managers-as-reviewers"></a>示例 5：人员经理作为审阅者

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```

因为`./manager`是相对查询，所以指定具有值`decisions`的 **queryRoot** 属性。

如果相应的访问评审 **范围** 面向具有共享通道的 B2B 直接连接用户和团队，则将分配团队所有者来评审 B2B 直接连接用户的访问权限。

## <a name="example-6-application-owners-as-reviewers"></a>示例 6：应用程序所有者作为审阅者

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
+ [试用教程](/graph/accessreviews-overview) ，了解如何使用访问评审 API 来评审对 Azure AD 资源的访问权限
+ [创建访问评审](/azure/active-directory/governance/create-access-review)
