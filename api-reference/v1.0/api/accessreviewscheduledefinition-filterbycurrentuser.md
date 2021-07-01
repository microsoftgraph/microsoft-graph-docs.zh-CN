---
title: accessReviewScheduleDefinition： filterByCurrentUser
description: 返回 accessReviewScheduleDefinition 对象，其中调用用户是审阅者。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2185e064dcd39049e90063dbcbe1100f9da36344
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209582"
---
# <a name="accessreviewscheduledefinition-filterbycurrentuser"></a><span data-ttu-id="61e62-103">accessReviewScheduleDefinition： filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="61e62-103">accessReviewScheduleDefinition: filterByCurrentUser</span></span>
<span data-ttu-id="61e62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61e62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61e62-105">返回 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象，其中调用用户是一个或多个 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="61e62-105">Returns [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects where the calling user is a reviewer on one or more [accessReviewInstance](../resources/accessreviewinstance.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="61e62-106">此 API 的默认页面大小为 100 accessReviewScheduleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="61e62-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="61e62-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="61e62-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="61e62-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="61e62-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="61e62-109">权限</span><span class="sxs-lookup"><span data-stu-id="61e62-109">Permissions</span></span>
<span data-ttu-id="61e62-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61e62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61e62-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="61e62-112">Permission type</span></span>|<span data-ttu-id="61e62-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61e62-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61e62-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61e62-114">Delegated (work or school account)</span></span>|<span data-ttu-id="61e62-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e62-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="61e62-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61e62-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61e62-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="61e62-117">Not supported.</span></span>|
|<span data-ttu-id="61e62-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="61e62-118">Application</span></span>|<span data-ttu-id="61e62-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e62-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61e62-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61e62-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61e62-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="61e62-121">Optional query parameters</span></span>
<span data-ttu-id="61e62-122">此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="61e62-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="61e62-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="61e62-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="61e62-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="61e62-124">Request headers</span></span>
|<span data-ttu-id="61e62-125">名称</span><span class="sxs-lookup"><span data-stu-id="61e62-125">Name</span></span>|<span data-ttu-id="61e62-126">说明</span><span class="sxs-lookup"><span data-stu-id="61e62-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="61e62-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="61e62-127">Authorization</span></span>|<span data-ttu-id="61e62-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61e62-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61e62-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="61e62-130">Request body</span></span>
<span data-ttu-id="61e62-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61e62-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61e62-132">响应</span><span class="sxs-lookup"><span data-stu-id="61e62-132">Response</span></span>

<span data-ttu-id="61e62-133">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="61e62-133">If successful, this function returns a `200 OK` response code and a [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61e62-134">示例</span><span class="sxs-lookup"><span data-stu-id="61e62-134">Examples</span></span>
<span data-ttu-id="61e62-135">返回调用用户是审阅者的所有审阅定义。</span><span class="sxs-lookup"><span data-stu-id="61e62-135">Returns all review definitions where the calling user is a reviewer.</span></span>

### <a name="request"></a><span data-ttu-id="61e62-136">请求</span><span class="sxs-lookup"><span data-stu-id="61e62-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="61e62-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="61e62-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewscheduledefinition_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[<span data-ttu-id="61e62-138">C#</span><span class="sxs-lookup"><span data-stu-id="61e62-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewscheduledefinition-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61e62-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61e62-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewscheduledefinition-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61e62-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61e62-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewscheduledefinition-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61e62-141">Java</span><span class="sxs-lookup"><span data-stu-id="61e62-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewscheduledefinition-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="61e62-142">响应</span><span class="sxs-lookup"><span data-stu-id="61e62-142">Response</span></span>
><span data-ttu-id="61e62-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="61e62-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewScheduleDefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewScheduleDefinition)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
            "id": "66666337-b075-4a92-9d71-255cc4b5d12a",
            "displayName": "All groups review",
            "createdDateTime": "2021-03-09T00:45:51.6272836Z",
            "lastModifiedDateTime": "2021-03-09T00:46:11.2041753Z",
            "status": "InProgress",
            "descriptionForAdmins": "All groups review",
            "descriptionForReviewers": "",
            "createdBy": {
                "id": "cae33dff-88e8-4e02-8a52-de021295997e",
                "displayName": "Example user",
                "userPrincipalName": "exampleuser@contoso.com"
            },
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "reviewers": [
                {
                    "query": "./owners",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": null
                }
            ],
            "fallbackReviewers": [],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": false,
                "defaultDecision": "None",
                "instanceDurationInDays": 3,
                "autoApplyDecisionsEnabled": true,
                "recommendationsEnabled": true,
                "recurrence": {
                    "pattern": {
                        "type": "weekly",
                        "interval": 1,
                        "month": 0,
                        "dayOfMonth": 0,
                        "daysOfWeek": [],
                        "firstDayOfWeek": "sunday",
                        "index": "first"
                    },
                    "range": {
                        "type": "numbered",
                        "numberOfOccurrences": 0,
                        "recurrenceTimeZone": null,
                        "startDate": "2021-03-09",
                        "endDate": "9999-12-31"
                    }
                },
                "applyActions": [
                    {
                        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                    }
                ]
            },
            "instances": []
        }
    ]
}
```
