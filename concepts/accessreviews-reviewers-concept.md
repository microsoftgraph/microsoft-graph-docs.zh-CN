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
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a><span data-ttu-id="c8450-103">使用 Microsoft Graph API 将审阅者分配给你的访问评审</span><span class="sxs-lookup"><span data-stu-id="c8450-103">Assign reviewers to your access review using the Microsoft Graph API</span></span>

<span data-ttu-id="c8450-104">Azure AD [访问评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 允许你以编程方式查看用户、服务主体或组对 Azure AD 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c8450-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

> [!NOTE]
> <span data-ttu-id="c8450-105">访问[评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)目前仅适用于 Microsoft Graph beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="c8450-105">The [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) is currently available in only the Microsoft Graph beta endpoint.</span></span> <span data-ttu-id="c8450-106">请勿在生产应用中使用它，因为它可能会随时更改，恕不另行通知。</span><span class="sxs-lookup"><span data-stu-id="c8450-106">Do not use it in production apps, as it is subject to change without notice.</span></span>

<span data-ttu-id="c8450-107">主要审阅者在访问评审 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)资源的 **reviewers** 属性中配置。</span><span class="sxs-lookup"><span data-stu-id="c8450-107">The primary reviewers are configured in the **reviewers** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) resource.</span></span>  <span data-ttu-id="c8450-108">此外，可以使用 **fallbackReviewers** 属性指定回退审阅者。</span><span class="sxs-lookup"><span data-stu-id="c8450-108">In addition, you can specify fallback reviewers by using **fallbackReviewers** property.</span></span> <span data-ttu-id="c8450-109">创建自审阅网站时，不需要 (查看自己的访问权限) 。</span><span class="sxs-lookup"><span data-stu-id="c8450-109">These properties are not required when you create a self-review (where users review their own access).</span></span>

## <a name="configure-reviewers"></a><span data-ttu-id="c8450-110">配置审阅者</span><span class="sxs-lookup"><span data-stu-id="c8450-110">Configure reviewers</span></span>

<span data-ttu-id="c8450-111">若要配置审阅者和回退审阅者，请设置 **accessReviewReviewerScope** 的 **query、queryRoot** 和 **queryType** 属性的值。 </span><span class="sxs-lookup"><span data-stu-id="c8450-111">To configure the reviewers and fallback reviewers, set the values of **query**, **queryRoot**, and **queryType** properties of **accessReviewReviewerScope**.</span></span> <span data-ttu-id="c8450-112">有关这些属性的说明，请参阅 [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true) 资源类型。</span><span class="sxs-lookup"><span data-stu-id="c8450-112">For descriptions of these properties, see [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true) resource type.</span></span>

### <a name="example-1-a-specific-user-as-the-reviewer"></a><span data-ttu-id="c8450-113">示例 1：作为审阅者的特定用户</span><span class="sxs-lookup"><span data-stu-id="c8450-113">Example 1: A specific user as the reviewer</span></span>

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-2-members-of-a-group-as-reviewers"></a><span data-ttu-id="c8450-114">示例 2：作为审阅者的组的成员</span><span class="sxs-lookup"><span data-stu-id="c8450-114">Example 2: Members of a group as reviewers</span></span>

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-group-owners-as-reviewers"></a><span data-ttu-id="c8450-115">示例 3：作为审阅者的组所有者</span><span class="sxs-lookup"><span data-stu-id="c8450-115">Example 3: Group owners as reviewers</span></span>
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

<span data-ttu-id="c8450-116">若要仅将特定国家/地区中的组所有者分配为审阅者，</span><span class="sxs-lookup"><span data-stu-id="c8450-116">To assign only the group owners from a specific country as reviewers:</span></span>

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

### <a name="example-4-people-managers-as-reviewers"></a><span data-ttu-id="c8450-117">示例 4：作为审阅者的人经理</span><span class="sxs-lookup"><span data-stu-id="c8450-117">Example 4: People managers as reviewers</span></span>

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```
<span data-ttu-id="c8450-118">由于 `./manager` 是相对查询，因此请用值 指定 **queryRoot** 属性 `decisions` 。</span><span class="sxs-lookup"><span data-stu-id="c8450-118">Because `./manager` is a relative query, specify the **queryRoot** property with the value `decisions`.</span></span>

## <a name="see-also"></a><span data-ttu-id="c8450-119">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c8450-119">See also</span></span>

+ [<span data-ttu-id="c8450-120">配置访问评审定义的范围</span><span class="sxs-lookup"><span data-stu-id="c8450-120">Configure the scope of your access review definition</span></span>](/graph/accessreviews-scope-concept)
