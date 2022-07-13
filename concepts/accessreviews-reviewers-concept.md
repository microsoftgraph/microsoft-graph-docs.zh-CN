---
title: 使用 Microsoft 图形 API 将审阅者分配到访问评审
description: 使用 Microsoft Graph 中的访问评审 API 分配访问评审者，例如特定用户、组的成员或所有者、人员管理器或应用所有者。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 72f5fd24e3949d9cb291e094006461c5c4e90b92
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768124"
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
        "query": "/users/{userId}",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="example-3-members-of-a-group-as-reviewers"></a>示例 3：组成员作为审阅者

```http
"reviewers": [
    {
        "query": "/groups/{groupId}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="example-4-group-owners-as-reviewers"></a>示例 4：组所有者作为审阅者

当访问评审的范围限定到组时，例如， [示例 1：查看分配给组的所有用户](accessreviews-scope-concept.md#example-1-review-all-users-assigned-to-a-group)， [示例 2：查看分配给组的所有来宾用户](accessreviews-scope-concept.md#example-2-review-all-guest-users-assigned-to-a-group)， [以及示例 3：查看分配给组的所有用户和组](accessreviews-scope-concept.md#example-3-review-all-users-and-groups-assigned-to-a-group)。
```http
"reviewers": [
    {
        "query": "/groups/{groupId}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

当访问评审的范围限定到组并仅将特定国家/地区的组所有者分配为审阅者时：

```http
"reviewers": [
    {
        "query": "/groups/{groupId}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

当访问评审范围限定到 *所有* 组时，例如示 [例 4：查看分配给所有 Microsoft 365 组的所有用户](accessreviews-scope-concept.md#example-4-review-all-users-assigned-to-all-microsoft-365-groups)， [示例 5：查看分配给所有 Microsoft 365 组的所有来宾用户](accessreviews-scope-concept.md#example-5-review-all-guest-users-assigned-to-all-microsoft-365-groups)， [以及示例 6：查看分配给所有团队的所有来宾用户](accessreviews-scope-concept.md#example-6-review-all-guest-users-assigned-to-all-teams)。

```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
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
        "query": "/servicePrincipals/{servicePrincipalId}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="next-steps"></a>后续步骤

+ [配置访问评审定义的范围](/graph/accessreviews-scope-concept)
+ [试用教程](/graph/accessreviews-overview) ，了解如何使用访问评审 API 来评审对 Azure AD 资源的访问权限
+ [创建访问评审](/azure/active-directory/governance/create-access-review)
