---
title: 列出 accessReviewInstanceDecisionItem 待审批
description: 检索调用用户等待审批的 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d1ce0293510f2f9a6ca526216b3fc2ad024b6285
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030472"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval-deprecated"></a><span data-ttu-id="0b38d-103">列出 accessReviewInstanceDecisionItems 待审批 (已弃) </span><span class="sxs-lookup"><span data-stu-id="0b38d-103">List accessReviewInstanceDecisionItems pending approval (deprecated)</span></span>

<span data-ttu-id="0b38d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b38d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="0b38d-105">此方法将弃用，并将于 2023 年 5 月 19 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="0b38d-105">This method will be deprecated and will stop returning data on May 19, 2023.</span></span> <span data-ttu-id="0b38d-106">它已被 [filterByCurrentUser 取代](accessreviewinstancedecisionitem-filterbycurrentuser.md)。</span><span class="sxs-lookup"><span data-stu-id="0b38d-106">It has been replaced by [filterByCurrentUser](accessreviewinstancedecisionitem-filterbycurrentuser.md).</span></span>

<span data-ttu-id="0b38d-107">检索[调用用户等待审批的特定 accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md)对象的[accessReviewInstance。](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0b38d-107">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects for a specific [accessReviewInstance](../resources/accessreviewscheduledefinition.md) pending approval by the calling user.</span></span> <span data-ttu-id="0b38d-108">返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括其所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="0b38d-108">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="0b38d-109">此 API 的默认页面大小为 100 accessReviewInstanceDecisionItem 对象。</span><span class="sxs-lookup"><span data-stu-id="0b38d-109">The default page size for this API is 100 accessReviewInstanceDecisionItem objects.</span></span> <span data-ttu-id="0b38d-110">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="0b38d-110">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="0b38d-111">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="0b38d-111">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b38d-112">权限</span><span class="sxs-lookup"><span data-stu-id="0b38d-112">Permissions</span></span>
<span data-ttu-id="0b38d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b38d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b38d-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b38d-115">Permission type</span></span>                        | <span data-ttu-id="0b38d-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b38d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b38d-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b38d-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b38d-118">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b38d-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="0b38d-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b38d-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b38d-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b38d-120">Not supported.</span></span>|

<span data-ttu-id="0b38d-121">登录用户还将仅在该决策实例的 accessReviewScheduleDefinition 中查看为其分配审阅者的决策。</span><span class="sxs-lookup"><span data-stu-id="0b38d-121">The signed-in user will also only see decisions of which they are assigned reviewer in that decision's instance's accessReviewScheduleDefinition.</span></span>

## <a name="http-request"></a><span data-ttu-id="0b38d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b38d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b38d-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b38d-123">Optional query parameters</span></span>
<span data-ttu-id="0b38d-124">此方法支持 `$skip` `$top` 和 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b38d-124">This method supports `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0b38d-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0b38d-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b38d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b38d-126">Request headers</span></span>
<span data-ttu-id="0b38d-127">无。</span><span class="sxs-lookup"><span data-stu-id="0b38d-127">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="0b38d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b38d-128">Request body</span></span>
<span data-ttu-id="0b38d-129">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b38d-129">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="0b38d-130">响应</span><span class="sxs-lookup"><span data-stu-id="0b38d-130">Response</span></span>
<span data-ttu-id="0b38d-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="0b38d-131">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b38d-132">示例</span><span class="sxs-lookup"><span data-stu-id="0b38d-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0b38d-133">请求</span><span class="sxs-lookup"><span data-stu-id="0b38d-133">Request</span></span>
<span data-ttu-id="0b38d-134">以下示例显示一个请求，请求检索有关访问评审实例的所有决策，等待调用用户批准。</span><span class="sxs-lookup"><span data-stu-id="0b38d-134">The following example shows a request to retrieve all the decisions on an instance of an access review pending the calling user's approval.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b38d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b38d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="0b38d-136">C#</span><span class="sxs-lookup"><span data-stu-id="0b38d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b38d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b38d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b38d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b38d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b38d-139">Java</span><span class="sxs-lookup"><span data-stu-id="0b38d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="0b38d-140">响应</span><span class="sxs-lookup"><span data-stu-id="0b38d-140">Response</span></span>
><span data-ttu-id="0b38d-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b38d-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 2,
    "value": [
        {
            "id": "654b34e7-b48f-4772-a2d4-08f1d0dd014c",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
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
                "userId": "7eae986b-d425-48b2-adf2-3c777f6256f3",
                "userDisplayName": "Adele Vance",
                "userPrincipalName": "AdeleV@contoso.com"
            }
        },
        {
            "id": "0311dba4-c60c-412e-ac77-14e1da23daf1",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
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
                "userId": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "userDisplayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="0b38d-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0b38d-142">See also</span></span>

- [<span data-ttu-id="0b38d-143">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="0b38d-143">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="0b38d-144">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="0b38d-144">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
