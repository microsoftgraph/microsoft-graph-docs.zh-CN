---
title: 教程：使用访问评审 API 查看对安全组的访问权限
description: 使用访问评审 API 查看对安全组的访问权限
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: b88c135c488b332814105dcab992e3a2a4ac465b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751130"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-your-security-groups"></a><span data-ttu-id="a6921-103">教程：使用访问评审 API 查看对安全组的访问权限</span><span class="sxs-lookup"><span data-stu-id="a6921-103">Tutorial: Use the access reviews API to review access to your security groups</span></span>

<span data-ttu-id="a6921-104">在本教程中，你将使用 Graph 资源管理器查看对租户中安全组的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a6921-104">In this tutorial, you will use Graph Explorer to review access to a security group in your tenant.</span></span>

<span data-ttu-id="a6921-105">可以使用浏览器Graph Postman 尝试和测试访问评审 API 调用，然后再将它们自动化到脚本或应用中。</span><span class="sxs-lookup"><span data-stu-id="a6921-105">You can use Graph Explorer or Postman to try out and test your access reviews API calls before you automate them into a script or an app.</span></span> <span data-ttu-id="a6921-106">这通过帮助您正确定义和验证查询而无需重复重新编译应用程序来节省时间。</span><span class="sxs-lookup"><span data-stu-id="a6921-106">This saves you time by helping you properly define and validate your queries without repeatedly recompiling your application.</span></span>

>[!NOTE]
><span data-ttu-id="a6921-107">为了可读性，本教程中显示的响应对象可能会缩短。</span><span class="sxs-lookup"><span data-stu-id="a6921-107">The response objects shown in this tutorial might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6921-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6921-108">Prerequisites</span></span>

<span data-ttu-id="a6921-109">若要完成本教程，需要以下资源和权限：</span><span class="sxs-lookup"><span data-stu-id="a6921-109">To complete this tutorial, you need the following resources and privileges:</span></span>

+ <span data-ttu-id="a6921-110">启用 Azure AD 或 EMS E5 许可证高级版 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="a6921-110">A working Azure AD tenant with an Azure AD Premium P2 or EMS E5 license enabled.</span></span>
+ <span data-ttu-id="a6921-111">以用户[Graph](https://developer.microsoft.com/graph/graph-explorer)登录资源管理器全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a6921-111">Log in to [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) as a user in a global administrator role.</span></span>
  + <span data-ttu-id="a6921-112">[可选]启动新的 **隐身** 或 **InPrivate** 浏览器会话或在匿名浏览器中启动会话。</span><span class="sxs-lookup"><span data-stu-id="a6921-112">[Optional] Start a new **incognito** or **InPrivate browser** session or start a session in an anonymous browser.</span></span> <span data-ttu-id="a6921-113">你将在本教程的稍后部分登录。</span><span class="sxs-lookup"><span data-stu-id="a6921-113">You will log in later in this tutorial.</span></span>
+ <span data-ttu-id="a6921-114">以下委派权限 `AccessReview.ReadWrite.All` `Group.ReadWrite.All` ：、。</span><span class="sxs-lookup"><span data-stu-id="a6921-114">The following delegated permissions: `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`.</span></span>

<span data-ttu-id="a6921-115">若要同意在浏览器浏览器中Graph权限：</span><span class="sxs-lookup"><span data-stu-id="a6921-115">To consent to the required permissions in Graph Explorer:</span></span>
1. <span data-ttu-id="a6921-116">选择用户帐户详细信息右边的设置齿轮图标，然后选择"**选择权限"。**</span><span class="sxs-lookup"><span data-stu-id="a6921-116">Select the settings gear icon to the right of the user account details, and then select **Select permissions**.</span></span>
   
   <span data-ttu-id="a6921-117">![选择 Microsoft Graph 权限](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
   </span><span class="sxs-lookup"><span data-stu-id="a6921-117">![Select the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Select the Microsoft Graph permissions":::-->

2. <span data-ttu-id="a6921-118">滚动浏览这些权限的权限列表：</span><span class="sxs-lookup"><span data-stu-id="a6921-118">Scroll through the list of permissions to these permissions:</span></span>
   + <span data-ttu-id="a6921-119">AccessReviews (3) ，展开，然后选择 **AccessReviews.ReadWrite.All**。</span><span class="sxs-lookup"><span data-stu-id="a6921-119">AccessReviews (3), expand and then select **AccessReviews.ReadWrite.All**.</span></span>
   + <span data-ttu-id="a6921-120">将 (2) ，展开，然后选择 **Group.ReadWrite.All。**</span><span class="sxs-lookup"><span data-stu-id="a6921-120">Group (2), expand and then select **Group.ReadWrite.All**.</span></span>
  
    <span data-ttu-id="a6921-121">选择 **"** 同意"，然后在弹出窗口中选择"代表你的组织同意"，然后选择"接受"接受权限同意。</span><span class="sxs-lookup"><span data-stu-id="a6921-121">Select **Consent**, and in the pop window, choose to **Consent on behalf of your organization** and then select **Accept** to accept the consent of the permissions.</span></span>
   
   <span data-ttu-id="a6921-122">![同意 Microsoft Graph权限](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png)
   </span><span class="sxs-lookup"><span data-stu-id="a6921-122">![Consent to the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png" alt-text="Consent to the Microsoft Graph permissions":::-->

## <a name="step-1-create-test-users-in-your-tenant"></a><span data-ttu-id="a6921-123">步骤 1：在租户内创建测试用户</span><span class="sxs-lookup"><span data-stu-id="a6921-123">Step 1: Create test users in your tenant</span></span>

<span data-ttu-id="a6921-124">通过运行下面的请求三次，每次更改 **displayName、mailNickname** 和 **userPrincipalName** 属性，创建三个新的测试用户。</span><span class="sxs-lookup"><span data-stu-id="a6921-124">Create three new test users by running the request below three times, changing the **displayName**, **mailNickname**, and **userPrincipalName** properties each time.</span></span> <span data-ttu-id="a6921-125">记录 **其 ID。**</span><span class="sxs-lookup"><span data-stu-id="a6921-125">Record their **id** s.</span></span>

### <a name="request"></a><span data-ttu-id="a6921-126">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-126">Request</span></span>

```http
POST /users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a><span data-ttu-id="a6921-127">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-127">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-create-a-security-group-assign-owners-and-add-members"></a><span data-ttu-id="a6921-128">步骤 2：创建安全组、分配所有者和添加成员</span><span class="sxs-lookup"><span data-stu-id="a6921-128">Step 2: Create a security group, assign owners, and add members</span></span>

<span data-ttu-id="a6921-129">创建一个名为 **"生成安全** 组"的安全组，该组是本教程中访问评审的目标。</span><span class="sxs-lookup"><span data-stu-id="a6921-129">Create a security group named **Building security group** that is the target of the access reviews in this tutorial.</span></span> <span data-ttu-id="a6921-130">为此组分配两个组所有者和两个成员。</span><span class="sxs-lookup"><span data-stu-id="a6921-130">Assign to this group two group owners and two members.</span></span> <span data-ttu-id="a6921-131">这些成员将是组所有者审查的主题。</span><span class="sxs-lookup"><span data-stu-id="a6921-131">These members will be the subject of review by the group owners.</span></span>

### <a name="request"></a><span data-ttu-id="a6921-132">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-132">Request</span></span>
<span data-ttu-id="a6921-133">在此调用中，替换：</span><span class="sxs-lookup"><span data-stu-id="a6921-133">In this call, replace:</span></span>
+ <span data-ttu-id="a6921-134">`010b2de0-0ed4-4ece-bfa2-22fff71d0497` 以及 `b828cc0e-4240-46ed-bb25-888744487e2d` 两 **个** 组所有者的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6921-134">`010b2de0-0ed4-4ece-bfa2-22fff71d0497` and `b828cc0e-4240-46ed-bb25-888744487e2d` with the **id** s of your two group owners.</span></span>
  + <span data-ttu-id="a6921-135">其中一 **个 ID** 属于你在步骤 1 中创建的用户之一。</span><span class="sxs-lookup"><span data-stu-id="a6921-135">One of the **id** s belongs to one of the users you created in Step 1.</span></span>
  + <span data-ttu-id="a6921-136">另一个是你的 **id**。若要检索 **id，** 请运行 `GET` `https://graph.microsoft.com/beta/me` 。</span><span class="sxs-lookup"><span data-stu-id="a6921-136">The other is your **id**. To retrieve your **id**, run `GET` on `https://graph.microsoft.com/beta/me`.</span></span>
+ <span data-ttu-id="a6921-137">`43b12b0c-ee2c-4257-96fe-505d823e06ab``859924d0-7115-422a-9ee8-ea8c0c014707`以及两个组的成员的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6921-137">`43b12b0c-ee2c-4257-96fe-505d823e06ab` and `859924d0-7115-422a-9ee8-ea8c0c014707` with the **id** s of you two group members.</span></span> <span data-ttu-id="a6921-138">这些是在步骤 1 中创建的其他两个成员。</span><span class="sxs-lookup"><span data-stu-id="a6921-138">These are the other two members you created in Step 1.</span></span>

```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Building security group",
    "displayName": "Building security group",
    "groupTypes": [],
    "mailEnabled": false,
    "mailNickname": "buildingsecurity",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/010b2de0-0ed4-4ece-bfa2-22fff71d0497",
        "https://graph.microsoft.com/beta/users/b828cc0e-4240-46ed-bb25-888744487e2d"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/43b12b0c-ee2c-4257-96fe-505d823e06ab",
        "https://graph.microsoft.com/beta/users/859924d0-7115-422a-9ee8-ea8c0c014707"
    ]
}
```

### <a name="response"></a><span data-ttu-id="a6921-139">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-139">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "825f1b5e-6fb2-4d9a-b393-d491101acc0c",
    "displayName": "Building security group",
    "groupTypes": []
}
```
<span data-ttu-id="a6921-140">在响应中，记录新组的 **ID，** 以在本教程的稍后部分使用它。</span><span class="sxs-lookup"><span data-stu-id="a6921-140">From the response, record the **id** of the new group to use it later in this tutorial.</span></span>

## <a name="step-3-create-an-access-review"></a><span data-ttu-id="a6921-141">步骤 3：创建访问评审</span><span class="sxs-lookup"><span data-stu-id="a6921-141">Step 3: Create an access review</span></span>

<span data-ttu-id="a6921-142">使用下列设置为安全组的成员创建访问评审：</span><span class="sxs-lookup"><span data-stu-id="a6921-142">Create an access review for members of the security group, using the following settings:</span></span>
+ <span data-ttu-id="a6921-143">这是一个自我审阅的访问评审。</span><span class="sxs-lookup"><span data-stu-id="a6921-143">It is a self-reviewing access review.</span></span> <span data-ttu-id="a6921-144">在这种情况下，被审阅的用户将自行证明其访问组的需求。</span><span class="sxs-lookup"><span data-stu-id="a6921-144">In this case, users under review will self-attest to their need for access to the group.</span></span>
+ <span data-ttu-id="a6921-145">这是一次访问评审。</span><span class="sxs-lookup"><span data-stu-id="a6921-145">This is a one-time access review.</span></span> <span data-ttu-id="a6921-146">在这种情况下，授予访问权限后，用户无需在访问评审期间再次自证明。</span><span class="sxs-lookup"><span data-stu-id="a6921-146">In this case, once access is granted, the user does not need to self-attest again within the access review period.</span></span>
+ <span data-ttu-id="a6921-147">审阅范围仅限于构建 **安全组 的成员**。</span><span class="sxs-lookup"><span data-stu-id="a6921-147">The review scope is limited to members of **Building security group**.</span></span>

### <a name="request"></a><span data-ttu-id="a6921-148">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-148">Request</span></span>
<span data-ttu-id="a6921-149">在此调用中，替换以下内容：</span><span class="sxs-lookup"><span data-stu-id="a6921-149">In this call, replace the following:</span></span>
+ <span data-ttu-id="a6921-150">`825f1b5e-6fb2-4d9a-b393-d491101acc0c`具有 **"生成\*\*\*\*安全组"的 ID。**</span><span class="sxs-lookup"><span data-stu-id="a6921-150">`825f1b5e-6fb2-4d9a-b393-d491101acc0c` with the **id** of **Building security group**.</span></span>
+ <span data-ttu-id="a6921-151">作用域指定将审阅应用于"生成安全"组 **的所有组的成员**。</span><span class="sxs-lookup"><span data-stu-id="a6921-151">The scope specifies that the review is applied to all group members of the the **Building security group**.</span></span> <span data-ttu-id="a6921-152">有关配置范围的更多选项，请参阅另 [请参阅部分](#see-also) 。</span><span class="sxs-lookup"><span data-stu-id="a6921-152">For more options for configuring the scope, see the [See also](#see-also) section.</span></span>
+ <span data-ttu-id="a6921-153">**startDate** 的值，其当前日期和 **endDate** 值，其日期为从开始日期起一年。</span><span class="sxs-lookup"><span data-stu-id="a6921-153">Value of **startDate** with today's date and value of **endDate** with a date one year from the start date.</span></span>

<span data-ttu-id="a6921-154">如果未能指定 **reviewers** 属性的值，则此访问评审被配置为具有审阅者的成员的自我审阅。</span><span class="sxs-lookup"><span data-stu-id="a6921-154">By failing to specify the value of the **reviewers** property, this access review is configured as self-reviewing with the members as the reviewers.</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "One-time self-review for members of Building security group",
    "descriptionForAdmins": "One-time self-review for members of Building security group",
    "descriptionForReviewers": "One-time self-review for members of Building security group",
    "scope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-09",
                "endDate": "2022-12-31"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

### <a name="response"></a><span data-ttu-id="a6921-155">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-155">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
    "id": "d7286a17-3a01-406a-b872-986b6b40317c",
    "displayName": "One-time self-review for members of Building security group",
    "status": "NotStarted",
    "createdBy": {
        "id": "b828cc0e-4240-46ed-bb25-888744487e2d",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "backupReviewers": [],
    "settings": {
        "defaultDecisionEnabled": false,
        "defaultDecision": "Deny",
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-09",
                "endDate": "2022-12-31"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

## <a name="step-4-list-instances-of-the-access-review"></a><span data-ttu-id="a6921-156">步骤 4：列出访问评审的实例</span><span class="sxs-lookup"><span data-stu-id="a6921-156">Step 4: List instances of the access review</span></span>

<span data-ttu-id="a6921-157">以下查询列出了访问评审定义的所有实例。</span><span class="sxs-lookup"><span data-stu-id="a6921-157">The following query lists all instances of the access review definition.</span></span> <span data-ttu-id="a6921-158">由于在步骤 3 中创建了一次访问评审，因此请求仅返回其 **id** 与访问定义的 id 相同的一 **个实例**。</span><span class="sxs-lookup"><span data-stu-id="a6921-158">Because you created a one-time access review in Step 3, the request returns only one instance whose **id** is the same as the access definition’s **id**.</span></span>

### <a name="request"></a><span data-ttu-id="a6921-159">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-159">Request</span></span>
<span data-ttu-id="a6921-160">在此调用中， `d7286a17-3a01-406a-b872-986b6b40317c` 将 替换为步骤 3 中返回的访问评审定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6921-160">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition returned in Step 3.</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c/instances
```

### <a name="response"></a><span data-ttu-id="a6921-161">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-161">Response</span></span>

<span data-ttu-id="a6921-162">在此响应中， **访问** 评审实例的状态是 `InProgress` **，因为 startDateTime** 已过去 **，endDateTime** 在将来。</span><span class="sxs-lookup"><span data-stu-id="a6921-162">In this response, the **status** of the access review instance is `InProgress` because **startDateTime** is past and **endDateTime** is in the future.</span></span> <span data-ttu-id="a6921-163">如果 **startDateTime** 在将来，则状态将为 `NotStarted` 。</span><span class="sxs-lookup"><span data-stu-id="a6921-163">If **startDateTime** is in the future, the status will be `NotStarted`.</span></span> <span data-ttu-id="a6921-164">另一方面，如果 **endDateTime** 过去，状态将为 `Completed` 。</span><span class="sxs-lookup"><span data-stu-id="a6921-164">On the other hand, if **endDateTime** is in the past, the status will be `Completed`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('d7286a17-3a01-406a-b872-986b6b40317c')/instances",
    "value": [
        {
            "id": "d7286a17-3a01-406a-b872-986b6b40317c",
            "startDateTime": "2021-02-10T15:09:40.153Z",
            "endDateTime": "2022-12-31T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```

## <a name="step-5-get-decisions"></a><span data-ttu-id="a6921-165">步骤 5：获取决策</span><span class="sxs-lookup"><span data-stu-id="a6921-165">Step 5: Get decisions</span></span>

<span data-ttu-id="a6921-166">您有兴趣做出有关访问评审实例的决策。</span><span class="sxs-lookup"><span data-stu-id="a6921-166">You are interested in the decisions taken for the instance of the access review.</span></span>

### <a name="request"></a><span data-ttu-id="a6921-167">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-167">Request</span></span>
<span data-ttu-id="a6921-168">在此调用中， `d7286a17-3a01-406a-b872-986b6b40317c` 将 替换为步骤 3 中返回的访问评审定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6921-168">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition returned in Step 3.</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c/instances/d7286a17-3a01-406a-b872-986b6b40317c/decisions
```

### <a name="response"></a><span data-ttu-id="a6921-169">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-169">Response</span></span>

<span data-ttu-id="a6921-170">以下响应显示为评价实例做出的决定。</span><span class="sxs-lookup"><span data-stu-id="a6921-170">The following response shows the decision taken for the instance of the review.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('d7286a17-3a01-406a-b872-986b6b40317c')/instances('d7286a17-3a01-406a-b872-986b6b40317c')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "1c74f500-9082-4dfe-80ac-784a6edb71d7",
            "accessReviewId": "d7286a17-3a01-406a-b872-986b6b40317c",
            "decision": "NotReviewed",
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
                "userDisplayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
                "displayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            }
        },
        {
            "id": "7744be81-7d17-40c9-8fd3-c9072b1ccace",
            "accessReviewId": "d7286a17-3a01-406a-b872-986b6b40317c",
            "decision": "NotReviewed",
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "859924d0-7115-422a-9ee8-ea8c0c014707",
                "userDisplayName": "Allan Deyoung",
                "userPrincipalName": "AllanD@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "859924d0-7115-422a-9ee8-ea8c0c014707",
                "displayName": "Allan Deyoung",
                "userPrincipalName": "AllanD@contoso.com"
            }
        }
    ]
}
```

<span data-ttu-id="a6921-171">在调用中 **，decision** 属性的值为 `NotReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="a6921-171">From the call, the **decision** property has the value of `NotReviewed`.</span></span> <span data-ttu-id="a6921-172">这是因为这两个成员都未完成自证明。</span><span class="sxs-lookup"><span data-stu-id="a6921-172">This is because none of the two members has completed their self-attestation.</span></span> <span data-ttu-id="a6921-173">按照步骤 6 了解每个成员如何自行证明其访问评审需求。</span><span class="sxs-lookup"><span data-stu-id="a6921-173">Follow step 6 to learn how each member can self-attest to their need for access review.</span></span>

## <a name="step-6-self-review-your-pending-access"></a><span data-ttu-id="a6921-174">步骤 6：自行查看待定访问权限</span><span class="sxs-lookup"><span data-stu-id="a6921-174">Step 6: Self-review your pending access</span></span>

<span data-ttu-id="a6921-175">在步骤 3 中，您将访问评审配置为自我审阅。</span><span class="sxs-lookup"><span data-stu-id="a6921-175">In Step 3, you configured the access review as a self-reviewing.</span></span> <span data-ttu-id="a6921-176">这意味着"生成安全"组的两个成员都必须自行证明其维护对组的访问权限需求。</span><span class="sxs-lookup"><span data-stu-id="a6921-176">This means that both members of **Building security group** must self-attest to their need to maintain access to the group.</span></span> <span data-ttu-id="a6921-177">您将以构建安全组的两个成员之一完成此步骤。</span><span class="sxs-lookup"><span data-stu-id="a6921-177">You will complete this step as one of the two members of Building security group.</span></span>

<span data-ttu-id="a6921-178">在此步骤中，您将执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a6921-178">In this step, you will:</span></span>
1. <span data-ttu-id="a6921-179">列出待处理的访问评审实例。</span><span class="sxs-lookup"><span data-stu-id="a6921-179">List your pending access review instances.</span></span>
2. <span data-ttu-id="a6921-180">完成访问评审自证明过程。</span><span class="sxs-lookup"><span data-stu-id="a6921-180">Complete the access review self-attestation process.</span></span>

<span data-ttu-id="a6921-181">在隐身或 **InPrivate** 浏览模式下，或通过匿名浏览器启动新的浏览器会话，并作为构建安全组的两个成员之 **一登录**。 </span><span class="sxs-lookup"><span data-stu-id="a6921-181">Start a new browser session in **incognito** or **InPrivate browsing** mode, or via an anonymous browser, and log in as one of the two members of **Building security group**.</span></span> <span data-ttu-id="a6921-182">这样，你将不会作为用户中断当前会话，全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a6921-182">By doing so, you will not interrupt your current session as a user in the global administrator role.</span></span> <span data-ttu-id="a6921-183">或者，你可以中断当前会话，Graph资源管理器中注销并作为两个组的成员之一重新登录。</span><span class="sxs-lookup"><span data-stu-id="a6921-183">Alternatively, you can interrupt your current session by logging out of Graph Explorer and logging back in as one of the two group members.</span></span>

### <a name="list-your-pending-access-review-instances"></a><span data-ttu-id="a6921-184">列出待处理的访问评审实例</span><span class="sxs-lookup"><span data-stu-id="a6921-184">List your pending access review instances</span></span>

<span data-ttu-id="a6921-185">在隐身浏览器会话和 Graph 资源管理器中，运行以下查询以列出待定访问评审实例：</span><span class="sxs-lookup"><span data-stu-id="a6921-185">In the incognito browser session and in Graph Explorer, run the following query to list your pending access review instances:</span></span>

#### <a name="request"></a><span data-ttu-id="a6921-186">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-186">Request</span></span>

```http
GET /me/pendingAccessReviewInstances
```

#### <a name="response"></a><span data-ttu-id="a6921-187">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-187">Response</span></span>
<span data-ttu-id="a6921-188">在下面的响应中，id 的用户 Alex  Wilber `43b12b0c-ee2c-4257-96fe-505d823e06ab` 有 1 个待自证明的访问评审。</span><span class="sxs-lookup"><span data-stu-id="a6921-188">From the response below, user Alex Wilber of **id** `43b12b0c-ee2c-4257-96fe-505d823e06ab` has 1 pending access review to self-attest to.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('43b12b0c-ee2c-4257-96fe-505d823e06ab')/pendingAccessReviewInstances",
    "@odata.count": 1,
    "value": [
        {
            "id": "d7286a17-3a01-406a-b872-986b6b40317c",
            "startDateTime": "2021-02-10T15:09:40.153Z",
            "endDateTime": "2022-12-31T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```
<span data-ttu-id="a6921-189">在用户 `/me/pendingAccessReviewInstances` 上下文中使用调用有很多优点：</span><span class="sxs-lookup"><span data-stu-id="a6921-189">Using the call `/me/pendingAccessReviewInstances` in a user context has a number of advantages:</span></span>
+ <span data-ttu-id="a6921-190">不需要任何服务主体。</span><span class="sxs-lookup"><span data-stu-id="a6921-190">No service principal is required.</span></span> <span data-ttu-id="a6921-191">用户可以调用和读取其挂起的访问评审操作。</span><span class="sxs-lookup"><span data-stu-id="a6921-191">A user can call and read their pending access review actions.</span></span>
+ <span data-ttu-id="a6921-192">小组件或 Intranet 页面上的插件，或作为后台服务运行的机器人或守护程序可以使用。</span><span class="sxs-lookup"><span data-stu-id="a6921-192">Can be used by widgets or plugins on an Intranet page, or a bot or daemon that run as a background service.</span></span> <span data-ttu-id="a6921-193">这些通知可以通知你新的访问评审或访问评审的更新。</span><span class="sxs-lookup"><span data-stu-id="a6921-193">These can notify you of new access reviews or of updates to access reviews.</span></span> 

### <a name="complete-the-access-review-self-attestation"></a><span data-ttu-id="a6921-194">完成访问评审自证明</span><span class="sxs-lookup"><span data-stu-id="a6921-194">Complete the access review self-attestation</span></span>

<span data-ttu-id="a6921-195">在同一个隐身浏览器会话中，登录 https://myaccess.microsoft.com/ 以完成自证明。</span><span class="sxs-lookup"><span data-stu-id="a6921-195">In the same incognito browser session, log in to https://myaccess.microsoft.com/ to complete the self-attestation.</span></span> <span data-ttu-id="a6921-196">从右侧导航栏中，选择 **访问评审** ，然后选择你的访问评审。</span><span class="sxs-lookup"><span data-stu-id="a6921-196">From the right navigation bar, select **access reviews** and choose your access review.</span></span> <span data-ttu-id="a6921-197">选择 **"是**，你仍然需要对构建安全 **组** 的访问权限"，输入原因，然后单击"提交 **"。**</span><span class="sxs-lookup"><span data-stu-id="a6921-197">Select **Yes**, that you still need access to **Building security group**, enter a reason, then click **Submit**.</span></span>

   <span data-ttu-id="a6921-198">![自证明访问评审](../images/../concepts/images/tutorial-accessreviews-api/selfattest.png)
   </span><span class="sxs-lookup"><span data-stu-id="a6921-198">![Self-attest to access review](../images/../concepts/images/tutorial-accessreviews-api/selfattest.png)
   </span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/selfattest.png" alt-text="Self-attest to access review":::-->

<span data-ttu-id="a6921-199">现在可以注销并退出无法识别的浏览器会话。</span><span class="sxs-lookup"><span data-stu-id="a6921-199">You can now logout and exit the incognito browser session.</span></span>

<span data-ttu-id="a6921-200">返回到你仍以全局管理员用户身份登录的主浏览器会话中，重复步骤 4 以查看已完成步骤 5 的成员的决策属性现在为 `Approve` 。</span><span class="sxs-lookup"><span data-stu-id="a6921-200">Back in the main browser session where you are still logged in as the global administrator user, repeat Step 4 to see that the **decision** property for the member who completed step 5 is now `Approve`.</span></span>

<span data-ttu-id="a6921-201">恭喜！</span><span class="sxs-lookup"><span data-stu-id="a6921-201">Congratulations!</span></span> <span data-ttu-id="a6921-202">你已创建访问评审并自行证明访问权限需求。</span><span class="sxs-lookup"><span data-stu-id="a6921-202">You have created an access review and self-attested to the need for access.</span></span> <span data-ttu-id="a6921-203">只需执行一次此操作，并保持访问权限，直到访问评审定义过期。</span><span class="sxs-lookup"><span data-stu-id="a6921-203">You only do this once, and maintain access until when the access review definition expires.</span></span>

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="a6921-204">第 7 步：清理资源</span><span class="sxs-lookup"><span data-stu-id="a6921-204">Step 7: Clean up resources</span></span>

<span data-ttu-id="a6921-205">删除为本教程创建的资源-**生成** 安全组、访问评审计划定义和三个测试用户。</span><span class="sxs-lookup"><span data-stu-id="a6921-205">Delete the resources that you created for this tutorial—**Building security group**, the access review schedule definition, and the three test users..</span></span>

### <a name="delete-the-security-group"></a><span data-ttu-id="a6921-206">删除安全组</span><span class="sxs-lookup"><span data-stu-id="a6921-206">Delete the security group</span></span>

#### <a name="request"></a><span data-ttu-id="a6921-207">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-207">Request</span></span>
<span data-ttu-id="a6921-208">在此调用中，将 `825f1b5e-6fb2-4d9a-b393-d491101acc0c` 替换为"生成 **安全\*\*\*\*组"的 ID。**</span><span class="sxs-lookup"><span data-stu-id="a6921-208">In this call, replace `825f1b5e-6fb2-4d9a-b393-d491101acc0c` with the **id** of **Building security group**.</span></span>

```http
DELETE https://graph.microsoft.com/beta/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c
```

#### <a name="response"></a><span data-ttu-id="a6921-209">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-209">Response</span></span>

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a><span data-ttu-id="a6921-210">删除访问评审定义</span><span class="sxs-lookup"><span data-stu-id="a6921-210">Delete the access review definition</span></span>

<span data-ttu-id="a6921-211">在此调用中， `d7286a17-3a01-406a-b872-986b6b40317c` 将 替换为 **访问** 评审定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6921-211">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition.</span></span> <span data-ttu-id="a6921-212">由于访问评审计划定义是访问评审的蓝图，删除该定义将删除与访问评审相关的设置、实例和决策。</span><span class="sxs-lookup"><span data-stu-id="a6921-212">Since the access review schedule definition is the blueprint for the access review, deleting the definition will remove the settings, instances, and decisions associated with the access review.</span></span>

#### <a name="request"></a><span data-ttu-id="a6921-213">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-213">Request</span></span>
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c
```

#### <a name="response"></a><span data-ttu-id="a6921-214">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-214">Response</span></span>
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-three-test-users"></a><span data-ttu-id="a6921-215">删除三个测试用户</span><span class="sxs-lookup"><span data-stu-id="a6921-215">Delete the three test users</span></span>

#### <a name="request"></a><span data-ttu-id="a6921-216">请求</span><span class="sxs-lookup"><span data-stu-id="a6921-216">Request</span></span>
<span data-ttu-id="a6921-217">在此调用中， `43b12b0c-ee2c-4257-96fe-505d823e06ab` 将 替换为 **测试** 用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6921-217">In this call, replace `43b12b0c-ee2c-4257-96fe-505d823e06ab` with the **id** of your test user.</span></span> <span data-ttu-id="a6921-218">对另外两个用户的 **ID** 重复这两次以删除它们。</span><span class="sxs-lookup"><span data-stu-id="a6921-218">Repeat this twice with the **id** s of the other two users to delete them.</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/43b12b0c-ee2c-4257-96fe-505d823e06ab
```

#### <a name="response"></a><span data-ttu-id="a6921-219">响应</span><span class="sxs-lookup"><span data-stu-id="a6921-219">Response</span></span>

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```


## <a name="see-also"></a><span data-ttu-id="a6921-220">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a6921-220">See also</span></span>

+ [<span data-ttu-id="a6921-221">访问评审 API 参考</span><span class="sxs-lookup"><span data-stu-id="a6921-221">Access reviews API Reference</span></span>](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="a6921-222">使用 Microsoft Graph API 配置访问评审定义的范围</span><span class="sxs-lookup"><span data-stu-id="a6921-222">Configure the scope of your access review definition using the Microsoft Graph API</span></span>](/graph/accessreviews-scope-concept)
+ [<span data-ttu-id="a6921-223">访问评审概述和许可证要求</span><span class="sxs-lookup"><span data-stu-id="a6921-223">Access reviews overview and license requirements</span></span>](/azure/active-directory/governance/access-reviews-overview)
+ [<span data-ttu-id="a6921-224">创建对应用程序应用程序的组&评审</span><span class="sxs-lookup"><span data-stu-id="a6921-224">Create an access review of groups & applications</span></span>](/azure/active-directory/governance/create-access-review)

