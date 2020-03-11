---
title: 创建 threatAssessmentRequest
description: 创建新的威胁评估请求。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44a8f786f4b492ae094c9b8ef12b9eff125d7218
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591528"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="2cfc0-103">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2cfc0-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="2cfc0-104">创建新的威胁评估请求。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-104">Create a new threat assessment request.</span></span>

<span data-ttu-id="2cfc0-105">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="2cfc0-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="2cfc0-106">邮件</span><span class="sxs-lookup"><span data-stu-id="2cfc0-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="2cfc0-107">电子邮件文件</span><span class="sxs-lookup"><span data-stu-id="2cfc0-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="2cfc0-108">文件</span><span class="sxs-lookup"><span data-stu-id="2cfc0-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="2cfc0-109">URL</span><span class="sxs-lookup"><span data-stu-id="2cfc0-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="2cfc0-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="2cfc0-110">Permissions</span></span>

<span data-ttu-id="2cfc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2cfc0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cfc0-113">Permission type</span></span>                        | <span data-ttu-id="2cfc0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cfc0-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2cfc0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cfc0-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="2cfc0-116">ThreatAssessment。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="2cfc0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cfc0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cfc0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-118">Not supported.</span></span>                              |
| <span data-ttu-id="2cfc0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cfc0-119">Application</span></span>                            | <span data-ttu-id="2cfc0-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-120">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="2cfc0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="2cfc0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cfc0-122">Request headers</span></span>

| <span data-ttu-id="2cfc0-123">名称</span><span class="sxs-lookup"><span data-stu-id="2cfc0-123">Name</span></span>          | <span data-ttu-id="2cfc0-124">说明</span><span class="sxs-lookup"><span data-stu-id="2cfc0-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2cfc0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cfc0-125">Authorization</span></span> | <span data-ttu-id="2cfc0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cfc0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cfc0-128">Request body</span></span>

<span data-ttu-id="2cfc0-129">在请求正文中，提供[threatAssessmentRequest](../resources/threatassessmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-129">In the request body, supply a JSON representation of a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2cfc0-130">响应</span><span class="sxs-lookup"><span data-stu-id="2cfc0-130">Response</span></span>

<span data-ttu-id="2cfc0-131">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[threatAssessmentRequest](../resources/threatassessmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-131">If successful, this method returns a `201 Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2cfc0-132">示例</span><span class="sxs-lookup"><span data-stu-id="2cfc0-132">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="2cfc0-133">示例1：创建邮件评估请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-133">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="2cfc0-134">请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-134">Request</span></span>

<span data-ttu-id="2cfc0-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_mailassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "spam",
  "messageUri": "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
}
```

#### <a name="response"></a><span data-ttu-id="2cfc0-136">响应</span><span class="sxs-lookup"><span data-stu-id="2cfc0-136">Response</span></span>

<span data-ttu-id="2cfc0-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-137">The following is an example of the response.</span></span>

> <span data-ttu-id="2cfc0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
  "messageUri": "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
  "createdBy": {
    "user": {
      "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin"
    }
  }
}
```

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="2cfc0-140">示例2：创建电子邮件评估请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-140">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="2cfc0-141">请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-141">Request</span></span>

<span data-ttu-id="2cfc0-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_emailfileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "malware",
  "contentData": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}
```

#### <a name="response"></a><span data-ttu-id="2cfc0-143">响应</span><span class="sxs-lookup"><span data-stu-id="2cfc0-143">Response</span></span>

<span data-ttu-id="2cfc0-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-144">The following is an example of the response.</span></span>

> <span data-ttu-id="2cfc0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="2cfc0-147">示例3：创建文件评估请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-147">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="2cfc0-148">请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-148">Request</span></span>

<span data-ttu-id="2cfc0-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_fileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.fileAssessmentRequest",
  "expectedAssessment": "block",
  "category": "malware",
  "fileName": "test.txt",
  "contentData": "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}
```

#### <a name="response"></a><span data-ttu-id="2cfc0-150">响应</span><span class="sxs-lookup"><span data-stu-id="2cfc0-150">Response</span></span>

<span data-ttu-id="2cfc0-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-151">The following is an example of the response.</span></span>

> <span data-ttu-id="2cfc0-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="2cfc0-154">示例4：创建 url 评估请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-154">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="2cfc0-155">请求</span><span class="sxs-lookup"><span data-stu-id="2cfc0-155">Request</span></span>

<span data-ttu-id="2cfc0-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_urlassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "url": "http://test.com",
  "expectedAssessment": "block",
  "category": "phishing"
}
```

#### <a name="response"></a><span data-ttu-id="2cfc0-157">响应</span><span class="sxs-lookup"><span data-stu-id="2cfc0-157">Response</span></span>

<span data-ttu-id="2cfc0-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-158">The following is an example of the response.</span></span>

> <span data-ttu-id="2cfc0-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2cfc0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
