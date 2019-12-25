---
title: 获取 threatAssessmentRequest
description: 检索指定的 threatassessmentrequest 对象的属性和关系。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fd5ee33d71c5019d6383ca31e5077b77cd4d40bc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867152"
---
# <a name="get-threatassessmentrequest"></a><span data-ttu-id="6799b-103">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6799b-103">Get threatAssessmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6799b-104">检索指定的[threatAssessmentRequest](../resources/threatassessmentrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6799b-104">Retrieve the properties and relationships of a specified [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

<span data-ttu-id="6799b-105">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="6799b-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="6799b-106">邮件</span><span class="sxs-lookup"><span data-stu-id="6799b-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="6799b-107">电子邮件文件</span><span class="sxs-lookup"><span data-stu-id="6799b-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="6799b-108">文件</span><span class="sxs-lookup"><span data-stu-id="6799b-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="6799b-109">URL</span><span class="sxs-lookup"><span data-stu-id="6799b-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="6799b-110">权限</span><span class="sxs-lookup"><span data-stu-id="6799b-110">Permissions</span></span>

<span data-ttu-id="6799b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6799b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6799b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6799b-113">Permission type</span></span>                        | <span data-ttu-id="6799b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6799b-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6799b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6799b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="6799b-116">ThreatAssessment。</span><span class="sxs-lookup"><span data-stu-id="6799b-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="6799b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6799b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6799b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6799b-118">Not supported.</span></span>                              |
| <span data-ttu-id="6799b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6799b-119">Application</span></span>                            | <span data-ttu-id="6799b-120">ThreatAssessment。</span><span class="sxs-lookup"><span data-stu-id="6799b-120">ThreatAssessment.Read.All.</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="6799b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6799b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6799b-122">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="6799b-122">Optional query parameters</span></span>

<span data-ttu-id="6799b-123">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6799b-123">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="6799b-124">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6799b-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="6799b-125">名称</span><span class="sxs-lookup"><span data-stu-id="6799b-125">Name</span></span>            |<span data-ttu-id="6799b-126">值</span><span class="sxs-lookup"><span data-stu-id="6799b-126">Value</span></span>    |<span data-ttu-id="6799b-127">说明</span><span class="sxs-lookup"><span data-stu-id="6799b-127">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6799b-128">$expand</span><span class="sxs-lookup"><span data-stu-id="6799b-128">$expand</span></span>         |<span data-ttu-id="6799b-129">string</span><span class="sxs-lookup"><span data-stu-id="6799b-129">string</span></span>   |<span data-ttu-id="6799b-130">在`$expand=results`查询中使用以检索威胁评估结果。</span><span class="sxs-lookup"><span data-stu-id="6799b-130">Using `$expand=results` in the query to retrieve the threat assessment result.</span></span>                                                                                              |
|<span data-ttu-id="6799b-131">$select</span><span class="sxs-lookup"><span data-stu-id="6799b-131">$select</span></span>         |<span data-ttu-id="6799b-132">string</span><span class="sxs-lookup"><span data-stu-id="6799b-132">string</span></span>   |<span data-ttu-id="6799b-p103">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="6799b-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |

## <a name="request-headers"></a><span data-ttu-id="6799b-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="6799b-135">Request headers</span></span>

| <span data-ttu-id="6799b-136">名称</span><span class="sxs-lookup"><span data-stu-id="6799b-136">Name</span></span>      |<span data-ttu-id="6799b-137">说明</span><span class="sxs-lookup"><span data-stu-id="6799b-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6799b-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="6799b-138">Authorization</span></span> | <span data-ttu-id="6799b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6799b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6799b-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="6799b-141">Request body</span></span>

<span data-ttu-id="6799b-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6799b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6799b-143">响应</span><span class="sxs-lookup"><span data-stu-id="6799b-143">Response</span></span>

<span data-ttu-id="6799b-144">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[threatAssessmentRequest](../resources/threatassessmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6799b-144">If successful, this method returns a `200 OK` response code and the requested [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span> <span data-ttu-id="6799b-145">返回该类型的属性： [mailAssessmentRequest](../resources/mailAssessmentRequest.md)、 [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)、 [fileAssessmentRequest](../resources/fileAssessmentRequest.md)、 [urlAssessmentRequest](../resources/urlAssessmentRequest.md)。</span><span class="sxs-lookup"><span data-stu-id="6799b-145">The properties of that type are returned: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span>

## <a name="examples"></a><span data-ttu-id="6799b-146">示例</span><span class="sxs-lookup"><span data-stu-id="6799b-146">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-mail-assessment-request"></a><span data-ttu-id="6799b-147">示例1：获取邮件评估请求的属性</span><span class="sxs-lookup"><span data-stu-id="6799b-147">Example 1: Get the properties of a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="6799b-148">请求</span><span class="sxs-lookup"><span data-stu-id="6799b-148">Request</span></span>

<span data-ttu-id="6799b-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6799b-149">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6799b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6799b-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6799b-151">C#</span><span class="sxs-lookup"><span data-stu-id="6799b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6799b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6799b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6799b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6799b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6799b-154">响应</span><span class="sxs-lookup"><span data-stu-id="6799b-154">Response</span></span>

<span data-ttu-id="6799b-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6799b-155">The following is an example of the response.</span></span>

> <span data-ttu-id="6799b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6799b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-the-properties-of-an-email-file-assessment-request"></a><span data-ttu-id="6799b-158">示例2：获取电子邮件文件评估请求的属性</span><span class="sxs-lookup"><span data-stu-id="6799b-158">Example 2: Get the properties of an email file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="6799b-159">请求</span><span class="sxs-lookup"><span data-stu-id="6799b-159">Request</span></span>

<span data-ttu-id="6799b-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6799b-160">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6799b-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="6799b-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailfileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6799b-162">C#</span><span class="sxs-lookup"><span data-stu-id="6799b-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailfileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6799b-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6799b-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailfileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6799b-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6799b-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailfileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6799b-165">响应</span><span class="sxs-lookup"><span data-stu-id="6799b-165">Response</span></span>

<span data-ttu-id="6799b-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6799b-166">The following is an example of the response.</span></span>

> <span data-ttu-id="6799b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6799b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-the-properties-of-a-file-assessment-request"></a><span data-ttu-id="6799b-169">示例3：获取文件评估请求的属性</span><span class="sxs-lookup"><span data-stu-id="6799b-169">Example 3: Get the properties of a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="6799b-170">请求</span><span class="sxs-lookup"><span data-stu-id="6799b-170">Request</span></span>

<span data-ttu-id="6799b-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6799b-171">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6799b-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="6799b-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6799b-173">C#</span><span class="sxs-lookup"><span data-stu-id="6799b-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6799b-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6799b-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6799b-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6799b-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6799b-176">响应</span><span class="sxs-lookup"><span data-stu-id="6799b-176">Response</span></span>

<span data-ttu-id="6799b-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6799b-177">The following is an example of the response.</span></span>

> <span data-ttu-id="6799b-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6799b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-get-the-properties-of-an-url-assessment-request"></a><span data-ttu-id="6799b-180">示例4：获取 url 评估请求的属性</span><span class="sxs-lookup"><span data-stu-id="6799b-180">Example 4: Get the properties of an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="6799b-181">请求</span><span class="sxs-lookup"><span data-stu-id="6799b-181">Request</span></span>

<span data-ttu-id="6799b-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6799b-182">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6799b-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="6799b-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_urlassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6799b-184">C#</span><span class="sxs-lookup"><span data-stu-id="6799b-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-urlassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6799b-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6799b-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-urlassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6799b-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6799b-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-urlassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6799b-187">响应</span><span class="sxs-lookup"><span data-stu-id="6799b-187">Response</span></span>

<span data-ttu-id="6799b-188">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6799b-188">The following is an example of the response.</span></span>

> <span data-ttu-id="6799b-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6799b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-expand-threat-assessment-results-for-a-request"></a><span data-ttu-id="6799b-191">示例5：展开请求的威胁评估结果</span><span class="sxs-lookup"><span data-stu-id="6799b-191">Example 5: Expand threat assessment results for a request</span></span>

#### <a name="request"></a><span data-ttu-id="6799b-192">请求</span><span class="sxs-lookup"><span data-stu-id="6799b-192">Request</span></span>

<span data-ttu-id="6799b-193">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6799b-193">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6799b-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="6799b-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest_expand_results"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996?$expand=results
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6799b-195">C#</span><span class="sxs-lookup"><span data-stu-id="6799b-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequest-expand-results-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6799b-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6799b-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequest-expand-results-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6799b-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6799b-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequest-expand-results-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6799b-198">响应</span><span class="sxs-lookup"><span data-stu-id="6799b-198">Response</span></span>

<span data-ttu-id="6799b-199">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6799b-199">The following is an example of the response.</span></span>

> <span data-ttu-id="6799b-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6799b-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
