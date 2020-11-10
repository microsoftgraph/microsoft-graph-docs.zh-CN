---
title: 创建 threatAssessmentRequest
description: 创建新的威胁评估请求。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4bf7996f84ade6668e6ce70720656158320af06a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952967"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="b231d-103">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="b231d-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="b231d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b231d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b231d-105">创建新的威胁评估请求。</span><span class="sxs-lookup"><span data-stu-id="b231d-105">Create a new threat assessment request.</span></span>

<span data-ttu-id="b231d-106">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="b231d-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="b231d-107">邮件</span><span class="sxs-lookup"><span data-stu-id="b231d-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="b231d-108">电子邮件文件</span><span class="sxs-lookup"><span data-stu-id="b231d-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="b231d-109">File</span><span class="sxs-lookup"><span data-stu-id="b231d-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="b231d-110">URL</span><span class="sxs-lookup"><span data-stu-id="b231d-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="b231d-111">权限</span><span class="sxs-lookup"><span data-stu-id="b231d-111">Permissions</span></span>

<span data-ttu-id="b231d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b231d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b231d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b231d-114">Permission type</span></span>                        | <span data-ttu-id="b231d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b231d-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b231d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b231d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b231d-117">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b231d-117">ThreatAssessment.ReadWrite.All</span></span>              |
| <span data-ttu-id="b231d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b231d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b231d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b231d-119">Not supported.</span></span>                              |
| <span data-ttu-id="b231d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b231d-120">Application</span></span>                            | <span data-ttu-id="b231d-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b231d-121">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="b231d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b231d-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="b231d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b231d-123">Request headers</span></span>

| <span data-ttu-id="b231d-124">名称</span><span class="sxs-lookup"><span data-stu-id="b231d-124">Name</span></span>          | <span data-ttu-id="b231d-125">说明</span><span class="sxs-lookup"><span data-stu-id="b231d-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b231d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b231d-126">Authorization</span></span> | <span data-ttu-id="b231d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b231d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b231d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b231d-129">Request body</span></span>

<span data-ttu-id="b231d-130">在请求正文中，提供 [threatAssessmentRequest](../resources/threatassessmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b231d-130">In the request body, supply a JSON representation of [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b231d-131">响应</span><span class="sxs-lookup"><span data-stu-id="b231d-131">Response</span></span>

<span data-ttu-id="b231d-132">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [threatAssessmentRequest](../resources/threatassessmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b231d-132">If successful, this method returns a `201, Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b231d-133">示例</span><span class="sxs-lookup"><span data-stu-id="b231d-133">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="b231d-134">示例1：创建邮件评估请求</span><span class="sxs-lookup"><span data-stu-id="b231d-134">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="b231d-135">请求</span><span class="sxs-lookup"><span data-stu-id="b231d-135">Request</span></span>

<span data-ttu-id="b231d-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b231d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b231d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b231d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "spam",
  "messageUri": "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
}
```
# <a name="c"></a>[<span data-ttu-id="b231d-138">C#</span><span class="sxs-lookup"><span data-stu-id="b231d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b231d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b231d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b231d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b231d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b231d-141">Java</span><span class="sxs-lookup"><span data-stu-id="b231d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b231d-142">响应</span><span class="sxs-lookup"><span data-stu-id="b231d-142">Response</span></span>

<span data-ttu-id="b231d-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b231d-143">The following is an example of the response.</span></span>

> <span data-ttu-id="b231d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b231d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="b231d-146">示例2：创建电子邮件评估请求</span><span class="sxs-lookup"><span data-stu-id="b231d-146">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="b231d-147">请求</span><span class="sxs-lookup"><span data-stu-id="b231d-147">Request</span></span>

<span data-ttu-id="b231d-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b231d-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b231d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b231d-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailfileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "malware",
  "contentData": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}
```
# <a name="c"></a>[<span data-ttu-id="b231d-150">C#</span><span class="sxs-lookup"><span data-stu-id="b231d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailfileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b231d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b231d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailfileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b231d-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b231d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailfileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b231d-153">Java</span><span class="sxs-lookup"><span data-stu-id="b231d-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailfileassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b231d-154">响应</span><span class="sxs-lookup"><span data-stu-id="b231d-154">Response</span></span>

<span data-ttu-id="b231d-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b231d-155">The following is an example of the response.</span></span>

> <span data-ttu-id="b231d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b231d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="b231d-158">示例3：创建文件评估请求</span><span class="sxs-lookup"><span data-stu-id="b231d-158">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="b231d-159">请求</span><span class="sxs-lookup"><span data-stu-id="b231d-159">Request</span></span>

<span data-ttu-id="b231d-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b231d-160">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b231d-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b231d-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_fileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.fileAssessmentRequest",
  "expectedAssessment": "block",
  "category": "malware",
  "fileName": "test.txt",
  "contentData": "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}
```
# <a name="c"></a>[<span data-ttu-id="b231d-162">C#</span><span class="sxs-lookup"><span data-stu-id="b231d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-fileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b231d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b231d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-fileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b231d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b231d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-fileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b231d-165">Java</span><span class="sxs-lookup"><span data-stu-id="b231d-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-fileassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b231d-166">响应</span><span class="sxs-lookup"><span data-stu-id="b231d-166">Response</span></span>

<span data-ttu-id="b231d-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b231d-167">The following is an example of the response.</span></span>

> <span data-ttu-id="b231d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b231d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="b231d-170">示例4：创建 url 评估请求</span><span class="sxs-lookup"><span data-stu-id="b231d-170">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="b231d-171">请求</span><span class="sxs-lookup"><span data-stu-id="b231d-171">Request</span></span>

<span data-ttu-id="b231d-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b231d-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b231d-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="b231d-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_urlassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "url": "http://test.com",
  "expectedAssessment": "block",
  "category": "phishing"
}
```
# <a name="c"></a>[<span data-ttu-id="b231d-174">C#</span><span class="sxs-lookup"><span data-stu-id="b231d-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-urlassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b231d-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b231d-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-urlassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b231d-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b231d-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-urlassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b231d-177">Java</span><span class="sxs-lookup"><span data-stu-id="b231d-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-urlassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b231d-178">响应</span><span class="sxs-lookup"><span data-stu-id="b231d-178">Response</span></span>

<span data-ttu-id="b231d-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b231d-179">The following is an example of the response.</span></span>

> <span data-ttu-id="b231d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b231d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "id": "8d87d2b2-ca4d-422c-f8df-08d774a5c9ac",
  "createdDateTime": "2019-11-29T08:26:09.8196703Z",
  "contentType": "url",
  "expectedAssessment": "block",
  "category": "phishing",
  "status": "pending",
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create threatAssessmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


