---
title: 获取 accessReviewScheduleDefinition
description: 读取 accessReviewScheduleDefinition 对象的属性和关系。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a5c6713d9fb99a7077888c903a61bfde12574a43
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030283"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="ecdd1-103">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="ecdd1-103">Get accessReviewScheduleDefinition</span></span>
<span data-ttu-id="ecdd1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecdd1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecdd1-105">读取 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-105">Read the properties and relationships of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="ecdd1-106">若要检索访问评审系列的实例，请使用 [列表 accessReviewInstance](accessreviewinstance-list.md) API。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-106">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>   

## <a name="permissions"></a><span data-ttu-id="ecdd1-107">权限</span><span class="sxs-lookup"><span data-stu-id="ecdd1-107">Permissions</span></span>
<span data-ttu-id="ecdd1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecdd1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecdd1-110">Permission type</span></span>|<span data-ttu-id="ecdd1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ecdd1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecdd1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecdd1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecdd1-113">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecdd1-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="ecdd1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecdd1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecdd1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-115">Not supported.</span></span>|
|<span data-ttu-id="ecdd1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecdd1-116">Application</span></span>|<span data-ttu-id="ecdd1-117">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecdd1-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="ecdd1-118">若要调用此 API，登录用户还必须位于允许其阅读访问评审的目录角色中，或者可以将该用户分配为访问评审的审阅者。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-118">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="ecdd1-119">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-119">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="ecdd1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecdd1-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecdd1-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ecdd1-121">Optional query parameters</span></span>
<span data-ttu-id="ecdd1-122">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-122">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="ecdd1-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecdd1-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecdd1-124">Request headers</span></span>
|<span data-ttu-id="ecdd1-125">名称</span><span class="sxs-lookup"><span data-stu-id="ecdd1-125">Name</span></span>|<span data-ttu-id="ecdd1-126">说明</span><span class="sxs-lookup"><span data-stu-id="ecdd1-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ecdd1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecdd1-127">Authorization</span></span>|<span data-ttu-id="ecdd1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecdd1-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecdd1-130">Request body</span></span>
<span data-ttu-id="ecdd1-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecdd1-132">响应</span><span class="sxs-lookup"><span data-stu-id="ecdd1-132">Response</span></span>

<span data-ttu-id="ecdd1-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-133">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecdd1-134">示例</span><span class="sxs-lookup"><span data-stu-id="ecdd1-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecdd1-135">请求</span><span class="sxs-lookup"><span data-stu-id="ecdd1-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewscheduledefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```


### <a name="response"></a><span data-ttu-id="ecdd1-136">响应</span><span class="sxs-lookup"><span data-stu-id="ecdd1-136">Response</span></span>
><span data-ttu-id="ecdd1-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ecdd1-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6bf2f6c-2f6c-d6bf-6c2f-bfd66c2fbfd6",
    "displayName": "Review example",
    "status": "Applying",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "reviewers": [
        {
            "query": "/v1.0/users/5555556e-fce3-4e2d-b28e-4ac0c7d2fa10",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [],
    "instanceEnumerationScope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": false,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 10,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-04-28",
                "endDate": "2021-05-08"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.disableAndDeleteUserApplyAction"
            }
        ]
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="ecdd1-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ecdd1-138">See also</span></span>

- [<span data-ttu-id="ecdd1-139">创建 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="ecdd1-139">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-post.md)
- [<span data-ttu-id="ecdd1-140">列出 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="ecdd1-140">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="ecdd1-141">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="ecdd1-141">List accessReviewInstance</span></span>](accessreviewinstance-list.md)
