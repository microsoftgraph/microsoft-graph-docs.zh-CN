---
title: 获取 threatAssessmentRequest
description: 检索指定的 threatassessmentrequest 对象的属性和关系。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6cf594cd40ce4e9c91b97706b970074ef7b34fa9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076587"
---
# <a name="get-threatassessmentrequest"></a><span data-ttu-id="e51e3-103">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e51e3-103">Get threatAssessmentRequest</span></span>

<span data-ttu-id="e51e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e51e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e51e3-105">检索指定的 [threatAssessmentRequest](../resources/threatassessmentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e51e3-105">Retrieve the properties and relationships of a specified [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

<span data-ttu-id="e51e3-106">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="e51e3-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="e51e3-107">邮件</span><span class="sxs-lookup"><span data-stu-id="e51e3-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="e51e3-108">电子邮件文件</span><span class="sxs-lookup"><span data-stu-id="e51e3-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="e51e3-109">File</span><span class="sxs-lookup"><span data-stu-id="e51e3-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="e51e3-110">URL</span><span class="sxs-lookup"><span data-stu-id="e51e3-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="e51e3-111">权限</span><span class="sxs-lookup"><span data-stu-id="e51e3-111">Permissions</span></span>

<span data-ttu-id="e51e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e51e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e51e3-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e51e3-114">Permission type</span></span>                        | <span data-ttu-id="e51e3-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e51e3-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e51e3-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e51e3-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e51e3-117">ThreatAssessment。</span><span class="sxs-lookup"><span data-stu-id="e51e3-117">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="e51e3-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e51e3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e51e3-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e51e3-119">Not supported.</span></span>                              |
| <span data-ttu-id="e51e3-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e51e3-120">Application</span></span>                            | <span data-ttu-id="e51e3-121">ThreatAssessment。</span><span class="sxs-lookup"><span data-stu-id="e51e3-121">ThreatAssessment.Read.All.</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="e51e3-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e51e3-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e51e3-123">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="e51e3-123">Optional query parameters</span></span>

<span data-ttu-id="e51e3-124">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e51e3-124">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="e51e3-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e51e3-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="e51e3-126">名称</span><span class="sxs-lookup"><span data-stu-id="e51e3-126">Name</span></span>            |<span data-ttu-id="e51e3-127">值</span><span class="sxs-lookup"><span data-stu-id="e51e3-127">Value</span></span>    |<span data-ttu-id="e51e3-128">说明</span><span class="sxs-lookup"><span data-stu-id="e51e3-128">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e51e3-129">$expand</span><span class="sxs-lookup"><span data-stu-id="e51e3-129">$expand</span></span>         |<span data-ttu-id="e51e3-130">string</span><span class="sxs-lookup"><span data-stu-id="e51e3-130">string</span></span>   |<span data-ttu-id="e51e3-131">`$expand=results`在查询中使用以检索威胁评估结果。</span><span class="sxs-lookup"><span data-stu-id="e51e3-131">Using `$expand=results` in the query to retrieve the threat assessment result.</span></span>                                                                                              |
|<span data-ttu-id="e51e3-132">$select</span><span class="sxs-lookup"><span data-stu-id="e51e3-132">$select</span></span>         |<span data-ttu-id="e51e3-133">string</span><span class="sxs-lookup"><span data-stu-id="e51e3-133">string</span></span>   |<span data-ttu-id="e51e3-p103">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="e51e3-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |

## <a name="request-headers"></a><span data-ttu-id="e51e3-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="e51e3-136">Request headers</span></span>

| <span data-ttu-id="e51e3-137">名称</span><span class="sxs-lookup"><span data-stu-id="e51e3-137">Name</span></span>      |<span data-ttu-id="e51e3-138">说明</span><span class="sxs-lookup"><span data-stu-id="e51e3-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e51e3-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="e51e3-139">Authorization</span></span> | <span data-ttu-id="e51e3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e51e3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e51e3-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="e51e3-142">Request body</span></span>

<span data-ttu-id="e51e3-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e51e3-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e51e3-144">响应</span><span class="sxs-lookup"><span data-stu-id="e51e3-144">Response</span></span>

<span data-ttu-id="e51e3-145">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [threatAssessmentRequest](../resources/threatassessmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e51e3-145">If successful, this method returns a `200 OK` response code and the requested [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span> <span data-ttu-id="e51e3-146">返回该类型的属性： [mailAssessmentRequest](../resources/mailAssessmentRequest.md)、 [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)、 [fileAssessmentRequest](../resources/fileAssessmentRequest.md)、 [urlAssessmentRequest](../resources/urlAssessmentRequest.md)。</span><span class="sxs-lookup"><span data-stu-id="e51e3-146">The properties of that type are returned: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span>

## <a name="examples"></a><span data-ttu-id="e51e3-147">示例</span><span class="sxs-lookup"><span data-stu-id="e51e3-147">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-mail-assessment-request"></a><span data-ttu-id="e51e3-148">示例1：获取邮件评估请求的属性</span><span class="sxs-lookup"><span data-stu-id="e51e3-148">Example 1: Get the properties of a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="e51e3-149">请求</span><span class="sxs-lookup"><span data-stu-id="e51e3-149">Request</span></span>

<span data-ttu-id="e51e3-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e51e3-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e51e3-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e51e3-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059
```
# <a name="c"></a>[<span data-ttu-id="e51e3-152">C#</span><span class="sxs-lookup"><span data-stu-id="e51e3-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e51e3-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e51e3-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e51e3-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e51e3-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e51e3-155">响应</span><span class="sxs-lookup"><span data-stu-id="e51e3-155">Response</span></span>

<span data-ttu-id="e51e3-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e51e3-156">The following is an example of the response.</span></span>

> <span data-ttu-id="e51e3-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e51e3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
  "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
  "createdDateTime": "2019-11-27T03:30:18.6890937Z",
  "contentType": "mail",
  "expectedAssessment": "block",
  "category": "spam",
  "status": "pending",
  "requestSource": "administrator",
  "recipientEmail": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com",
  "destinationRoutingReason": "notJunk",
  "messageUri": "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
  "createdBy": {
    "user": {
      "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin"
    }
  }
}
```

### <a name="example-2-get-the-properties-of-an-email-file-assessment-request"></a><span data-ttu-id="e51e3-159">示例2：获取电子邮件文件评估请求的属性</span><span class="sxs-lookup"><span data-stu-id="e51e3-159">Example 2: Get the properties of an email file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="e51e3-160">请求</span><span class="sxs-lookup"><span data-stu-id="e51e3-160">Request</span></span>

<span data-ttu-id="e51e3-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e51e3-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e51e3-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="e51e3-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailfileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf
```
# <a name="c"></a>[<span data-ttu-id="e51e3-163">C#</span><span class="sxs-lookup"><span data-stu-id="e51e3-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailfileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e51e3-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e51e3-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailfileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e51e3-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e51e3-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailfileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e51e3-166">响应</span><span class="sxs-lookup"><span data-stu-id="e51e3-166">Response</span></span>

<span data-ttu-id="e51e3-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e51e3-167">The following is an example of the response.</span></span>

> <span data-ttu-id="e51e3-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e51e3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
  "id": "ab2ad9b3-2213-4091-ae0c-08d76ddbcacf",
  "createdDateTime": "2019-11-20T17:05:06.4088076Z",
  "contentType": "mail",
  "expectedAssessment": "block",
  "category": "malware",
  "status": "completed",
  "requestSource": "administrator",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "destinationRoutingReason": "notJunk",
  "contentData": "",
  "createdBy": {
    "user": {
      "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin"
    }
  }
}
```

### <a name="example-3-get-the-properties-of-a-file-assessment-request"></a><span data-ttu-id="e51e3-170">示例3：获取文件评估请求的属性</span><span class="sxs-lookup"><span data-stu-id="e51e3-170">Example 3: Get the properties of a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="e51e3-171">请求</span><span class="sxs-lookup"><span data-stu-id="e51e3-171">Request</span></span>

<span data-ttu-id="e51e3-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e51e3-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e51e3-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="e51e3-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa
```
# <a name="c"></a>[<span data-ttu-id="e51e3-174">C#</span><span class="sxs-lookup"><span data-stu-id="e51e3-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e51e3-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e51e3-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e51e3-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e51e3-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e51e3-177">响应</span><span class="sxs-lookup"><span data-stu-id="e51e3-177">Response</span></span>

<span data-ttu-id="e51e3-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e51e3-178">The following is an example of the response.</span></span>

> <span data-ttu-id="e51e3-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e51e3-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
  "@odata.type": "#microsoft.graph.fileAssessmentRequest",
  "id": "18406a56-7209-4720-a250-08d772fccdaa",
  "createdDateTime": "2019-11-27T05:44:00.4051536Z",
  "contentType": "file",
  "expectedAssessment": "block",
  "category": "malware",
  "status": "completed",
  "requestSource": "administrator",
  "fileName": "b3d5b715-4b88-4bbb-b0ae-9a9281a3f18a.csv",
  "contentData": "",
  "createdBy": {
    "user": {
      "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin"
    }
  }
}
```

### <a name="example-4-get-the-properties-of-an-url-assessment-request"></a><span data-ttu-id="e51e3-181">示例4：获取 url 评估请求的属性</span><span class="sxs-lookup"><span data-stu-id="e51e3-181">Example 4: Get the properties of an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="e51e3-182">请求</span><span class="sxs-lookup"><span data-stu-id="e51e3-182">Request</span></span>

<span data-ttu-id="e51e3-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e51e3-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e51e3-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="e51e3-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_urlassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b
```
# <a name="c"></a>[<span data-ttu-id="e51e3-185">C#</span><span class="sxs-lookup"><span data-stu-id="e51e3-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-urlassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e51e3-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e51e3-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-urlassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e51e3-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e51e3-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-urlassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e51e3-188">响应</span><span class="sxs-lookup"><span data-stu-id="e51e3-188">Response</span></span>

<span data-ttu-id="e51e3-189">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e51e3-189">The following is an example of the response.</span></span>

> <span data-ttu-id="e51e3-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e51e3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "id": "723c35be-8b5a-47ae-29c0-08d76ddb7f5b",
  "createdDateTime": "2019-11-20T17:02:59.8160832Z",
  "contentType": "url",
  "expectedAssessment": "unblock",
  "category": "phishing",
  "status": "completed",
  "requestSource": "administrator",
  "url": "http://test.com",
  "createdBy": {
    "user": {
      "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin"
    }
  }
}
```

### <a name="example-5-expand-threat-assessment-results-for-a-request"></a><span data-ttu-id="e51e3-192">示例5：展开请求的威胁评估结果</span><span class="sxs-lookup"><span data-stu-id="e51e3-192">Example 5: Expand threat assessment results for a request</span></span>

#### <a name="request"></a><span data-ttu-id="e51e3-193">请求</span><span class="sxs-lookup"><span data-stu-id="e51e3-193">Request</span></span>

<span data-ttu-id="e51e3-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e51e3-194">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e51e3-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="e51e3-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest_expand_results"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996?$expand=results
```
# <a name="c"></a>[<span data-ttu-id="e51e3-196">C#</span><span class="sxs-lookup"><span data-stu-id="e51e3-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequest-expand-results-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e51e3-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e51e3-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequest-expand-results-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e51e3-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e51e3-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequest-expand-results-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e51e3-199">响应</span><span class="sxs-lookup"><span data-stu-id="e51e3-199">Response</span></span>

<span data-ttu-id="e51e3-200">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e51e3-200">The following is an example of the response.</span></span>

> <span data-ttu-id="e51e3-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e51e3-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests(results())/$entity",
    "@odata.type": "#microsoft.graph.mailAssessmentRequest",
    "id": "11922306-b25b-4605-ff0d-08d772fcf996",
    "createdDateTime": "2019-11-27T05:45:14.0962061Z",
    "contentType": "mail",
    "expectedAssessment": "block",
    "category": "phishing",
    "status": "completed",
    "requestSource": "administrator",
    "recipientEmail": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com",
    "destinationRoutingReason": "notJunk",
    "messageUri": "",
    "createdBy": {
      "user": {
        "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
        "displayName": "Ronald Admin"
      }
    },
    "results@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests('11922306-b25b-4605-ff0d-08d772fcf996')/microsoft.graph.mailAssessmentRequest/results",
    "results": [
        {
            "id": "63798129-a62c-4f9e-2c6d-08d772fcfb0e",
            "createdDateTime": "2019-11-27T05:45:16.55Z",
            "resultType": "checkPolicy",
            "message": "No policy was hit."
        },
        {
            "id": "d38c2448-79eb-467e-2495-08d772fdb7d1",
            "createdDateTime": "2019-11-27T05:50:33.243Z",
            "resultType": "rescan",
            "message": "Not Spam"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get threatAssessmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


