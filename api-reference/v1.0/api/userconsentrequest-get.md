---
title: 获取 userConsentRequest
description: 读取 userConsentRequest 对象的属性和关系。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 921600ae2200428eae7ea5ed9b58e3c2c1e5f11c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51506933"
---
# <a name="get-userconsentrequest"></a><span data-ttu-id="226ec-103">获取 userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="226ec-103">Get userConsentRequest</span></span>

<span data-ttu-id="226ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="226ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="226ec-105">读取 [userConsentRequest](../resources/userconsentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="226ec-105">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="226ec-106">权限</span><span class="sxs-lookup"><span data-stu-id="226ec-106">Permissions</span></span>

<span data-ttu-id="226ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="226ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="226ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="226ec-109">Permission type</span></span>|<span data-ttu-id="226ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="226ec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="226ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="226ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="226ec-112">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="226ec-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="226ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="226ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="226ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="226ec-114">Not supported.</span></span>|
|<span data-ttu-id="226ec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="226ec-115">Application</span></span>|<span data-ttu-id="226ec-116">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="226ec-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="226ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="226ec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{appconsentrequest-id}/userConsentRequests/{userconsentrequest-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="226ec-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="226ec-118">Optional query parameters</span></span>

<span data-ttu-id="226ec-119">此方法支持  `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="226ec-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="226ec-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="226ec-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="226ec-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="226ec-121">Request headers</span></span>

|<span data-ttu-id="226ec-122">名称</span><span class="sxs-lookup"><span data-stu-id="226ec-122">Name</span></span>|<span data-ttu-id="226ec-123">说明</span><span class="sxs-lookup"><span data-stu-id="226ec-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="226ec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="226ec-124">Authorization</span></span>|<span data-ttu-id="226ec-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="226ec-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="226ec-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="226ec-127">Request body</span></span>

<span data-ttu-id="226ec-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="226ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="226ec-129">响应</span><span class="sxs-lookup"><span data-stu-id="226ec-129">Response</span></span>

<span data-ttu-id="226ec-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userConsentRequest](../resources/userconsentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="226ec-130">If successful, this method returns a `200 OK` response code and a [userConsentRequest](../resources/userconsentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="226ec-131">示例</span><span class="sxs-lookup"><span data-stu-id="226ec-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="226ec-132">请求</span><span class="sxs-lookup"><span data-stu-id="226ec-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="226ec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="226ec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/acef2660-d194-4943-b927-4fe4fb5cb7e3
```
# <a name="c"></a>[<span data-ttu-id="226ec-134">C#</span><span class="sxs-lookup"><span data-stu-id="226ec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userconsentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="226ec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="226ec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userconsentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="226ec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="226ec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userconsentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="226ec-137">Java</span><span class="sxs-lookup"><span data-stu-id="226ec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userconsentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="226ec-138">响应</span><span class="sxs-lookup"><span data-stu-id="226ec-138">Response</span></span>

<span data-ttu-id="226ec-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="226ec-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userConsentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests",
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
  "approval@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/$entity",
  "approval": {
    "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
    "stages@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/stages",
    "stages": [
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
```
