---
title: userConsentRequests：filterByCurrentUser
description: 检索当前用户是审阅者的 userConsentRequests。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ddef281b50a4a60895f141b433289a2fc3e8a1d3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201857"
---
# <a name="userconsentrequests-filterbycurrentuser"></a><span data-ttu-id="6f352-103">userConsentRequests：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="6f352-103">userConsentRequests: filterByCurrentUser</span></span>
<span data-ttu-id="6f352-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f352-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f352-105">检索 [appConsentRequest 的 userConsentRequest，](../resources/userconsentrequest.md) 当前用户是审阅者，并且 userConsentRequest 的状态为 `InProgress` 。</span><span class="sxs-lookup"><span data-stu-id="6f352-105">Retrieve the [userConsentRequests](../resources/userconsentrequest.md) for an appConsentRequest for which the current user is the reviewer and the status of the userConsentRequest is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f352-106">权限</span><span class="sxs-lookup"><span data-stu-id="6f352-106">Permissions</span></span>
<span data-ttu-id="6f352-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f352-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f352-109">Permission type</span></span>|<span data-ttu-id="6f352-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f352-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f352-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f352-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f352-112">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f352-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="6f352-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f352-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f352-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f352-114">Not supported.</span></span>|
|<span data-ttu-id="6f352-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f352-115">Application</span></span>|<span data-ttu-id="6f352-116">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f352-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f352-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f352-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}/userConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="6f352-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="6f352-118">Function parameters</span></span>
<span data-ttu-id="6f352-119">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="6f352-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6f352-120">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="6f352-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6f352-121">属性</span><span class="sxs-lookup"><span data-stu-id="6f352-121">Property</span></span>|<span data-ttu-id="6f352-122">类型</span><span class="sxs-lookup"><span data-stu-id="6f352-122">Type</span></span>|<span data-ttu-id="6f352-123">说明</span><span class="sxs-lookup"><span data-stu-id="6f352-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f352-124">on</span><span class="sxs-lookup"><span data-stu-id="6f352-124">on</span></span>|<span data-ttu-id="6f352-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="6f352-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="6f352-126">筛选以查询当前用户是审阅者的 appConsentRequest 的 userConsentRequests。</span><span class="sxs-lookup"><span data-stu-id="6f352-126">Filter to query userConsentRequests for an appConsentRequest for which the current user is a reviewer.</span></span> <span data-ttu-id="6f352-127">允许的值为 `reviewer` 。</span><span class="sxs-lookup"><span data-stu-id="6f352-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="6f352-128">必需。</span><span class="sxs-lookup"><span data-stu-id="6f352-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="6f352-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6f352-129">Optional query parameters</span></span>
<span data-ttu-id="6f352-130">此函数支持  `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6f352-130">This function supports the `$filter` OData query parameter to help customize the response.</span></span> <span data-ttu-id="6f352-131">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6f352-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f352-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f352-132">Request headers</span></span>
|<span data-ttu-id="6f352-133">名称</span><span class="sxs-lookup"><span data-stu-id="6f352-133">Name</span></span>|<span data-ttu-id="6f352-134">说明</span><span class="sxs-lookup"><span data-stu-id="6f352-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f352-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f352-135">Authorization</span></span>|<span data-ttu-id="6f352-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f352-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f352-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f352-138">Request body</span></span>
<span data-ttu-id="6f352-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f352-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f352-140">响应</span><span class="sxs-lookup"><span data-stu-id="6f352-140">Response</span></span>

<span data-ttu-id="6f352-141">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userConsentRequest](../resources/userconsentrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6f352-141">If successful, this method returns a `200 OK` response code and a collection of [userConsentRequest](../resources/userconsentrequest.md) objects in the response body.</span></span>

## <a name="example-list-all-userconsentrequests-for-which-the-current-user-is-the-reviewer-and-the-status-is-completed"></a><span data-ttu-id="6f352-142">示例：列出当前用户是审阅者且状态为"已完成"的 userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="6f352-142">Example: List all userConsentRequests for which the current user is the reviewer and the status is Completed</span></span>

### <a name="request"></a><span data-ttu-id="6f352-143">请求</span><span class="sxs-lookup"><span data-stu-id="6f352-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6f352-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f352-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')?$filter= (status eq 'Completed')
```
# <a name="c"></a>[<span data-ttu-id="6f352-145">C#</span><span class="sxs-lookup"><span data-stu-id="6f352-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f352-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f352-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f352-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f352-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f352-148">Java</span><span class="sxs-lookup"><span data-stu-id="6f352-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6f352-149">响应</span><span class="sxs-lookup"><span data-stu-id="6f352-149">Response</span></span>
<span data-ttu-id="6f352-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6f352-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userConsentRequest)",
    "@odata.count": 1,
    "value": [
      {
      "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
      "reason": "I need access",
      "status": "Completed",
      "createdDateTime": "2019-10-18T19:07:19.7374554Z",
      "createdBy": {
        "user": {
          "id": "db60ab61-caea-4889-a824-98de31ef31b5",
          "displayName": "Alex Wilber",
          "userPrincipalName": "AlexW@contoso.com",
          "mail": "AlexW@contoso.com"
        }
      },
      "approval@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/$entity",
      "approval": {
        "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
        "steps@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/steps",
        "steps": [
          {
            "id": "f5a4ca4a-1316-4872-8112-993c55dab51e",
            "displayName": null,
            "reviewedDateTime": "2019-10-19T04:12:09.633Z",
            "reviewResult": "Approve",
            "status": "Completed",
            "assignedToMe": true,
            "justification": "Admin consent granted.",
            "reviewedBy": {
              "id": "00000001-0000-0000-c000-000000000000",
              "displayName": "",
              "userPrincipalName": "",
              "mail": ""
            }
          }
        ]
      },
      "approvalId": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
      "completedDateTime": null,
      "customData": null
    }
  ]
}
```
