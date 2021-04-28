---
title: 列出 threatAssessmentRequests
description: 检索 threatassessmentrequest 对象的列表。
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: fb5e804682741c79d8ea3daeca5e6512575c16de
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039564"
---
# <a name="list-threatassessmentrequests"></a><span data-ttu-id="5491c-103">列出 threatAssessmentRequests</span><span class="sxs-lookup"><span data-stu-id="5491c-103">List threatAssessmentRequests</span></span>

<span data-ttu-id="5491c-104">检索 [threatAssessmentRequest 对象](../resources/threatassessmentrequest.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="5491c-104">Retrieve a list of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects.</span></span>

<span data-ttu-id="5491c-105">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="5491c-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="5491c-106">邮件</span><span class="sxs-lookup"><span data-stu-id="5491c-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="5491c-107">电子邮件文件</span><span class="sxs-lookup"><span data-stu-id="5491c-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="5491c-108">文件</span><span class="sxs-lookup"><span data-stu-id="5491c-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="5491c-109">URL</span><span class="sxs-lookup"><span data-stu-id="5491c-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="5491c-110">权限</span><span class="sxs-lookup"><span data-stu-id="5491c-110">Permissions</span></span>

<span data-ttu-id="5491c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5491c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5491c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="5491c-113">Permission type</span></span>                        | <span data-ttu-id="5491c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5491c-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5491c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5491c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="5491c-116">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5491c-116">ThreatAssessment.ReadWrite.All</span></span>             |
| <span data-ttu-id="5491c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5491c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5491c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5491c-118">Not supported.</span></span>                              |
| <span data-ttu-id="5491c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="5491c-119">Application</span></span>                            | <span data-ttu-id="5491c-120">ThreatAssessment.Read.All</span><span class="sxs-lookup"><span data-stu-id="5491c-120">ThreatAssessment.Read.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="5491c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5491c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5491c-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5491c-122">Optional query parameters</span></span>

<span data-ttu-id="5491c-123">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5491c-123">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="5491c-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5491c-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="5491c-125">名称</span><span class="sxs-lookup"><span data-stu-id="5491c-125">Name</span></span>            |<span data-ttu-id="5491c-126">值</span><span class="sxs-lookup"><span data-stu-id="5491c-126">Value</span></span>    |<span data-ttu-id="5491c-127">说明</span><span class="sxs-lookup"><span data-stu-id="5491c-127">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5491c-128">$filter</span><span class="sxs-lookup"><span data-stu-id="5491c-128">$filter</span></span>         |<span data-ttu-id="5491c-129">string</span><span class="sxs-lookup"><span data-stu-id="5491c-129">string</span></span>   |<span data-ttu-id="5491c-130">将响应限制到仅包含指定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="5491c-130">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="5491c-131">$orderby</span><span class="sxs-lookup"><span data-stu-id="5491c-131">$orderby</span></span>        |<span data-ttu-id="5491c-132">string</span><span class="sxs-lookup"><span data-stu-id="5491c-132">string</span></span>   |<span data-ttu-id="5491c-133">默认情况下，响应中的对象按 **其 createdDateTime** 值降序排序。</span><span class="sxs-lookup"><span data-stu-id="5491c-133">By default, the objects in the response are descending ordered by their **createdDateTime** value.</span></span>                                                                          |
|<span data-ttu-id="5491c-134">$select</span><span class="sxs-lookup"><span data-stu-id="5491c-134">$select</span></span>         |<span data-ttu-id="5491c-135">string</span><span class="sxs-lookup"><span data-stu-id="5491c-135">string</span></span>   |<span data-ttu-id="5491c-p103">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="5491c-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="5491c-138">$skipToken</span><span class="sxs-lookup"><span data-stu-id="5491c-138">$skipToken</span></span>      |<span data-ttu-id="5491c-139">string</span><span class="sxs-lookup"><span data-stu-id="5491c-139">string</span></span>   |<span data-ttu-id="5491c-140">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="5491c-140">Retrieves the next page of results from result sets that span multiple pages.</span></span>                                                                                               |

## <a name="request-headers"></a><span data-ttu-id="5491c-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="5491c-141">Request headers</span></span>

| <span data-ttu-id="5491c-142">名称</span><span class="sxs-lookup"><span data-stu-id="5491c-142">Name</span></span>      |<span data-ttu-id="5491c-143">说明</span><span class="sxs-lookup"><span data-stu-id="5491c-143">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5491c-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="5491c-144">Authorization</span></span> | <span data-ttu-id="5491c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5491c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5491c-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="5491c-147">Request body</span></span>

<span data-ttu-id="5491c-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5491c-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5491c-149">响应</span><span class="sxs-lookup"><span data-stu-id="5491c-149">Response</span></span>

<span data-ttu-id="5491c-150">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [threatAssessmentRequest](../resources/threatassessmentrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5491c-150">If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5491c-151">示例</span><span class="sxs-lookup"><span data-stu-id="5491c-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5491c-152">请求</span><span class="sxs-lookup"><span data-stu-id="5491c-152">Request</span></span>

<span data-ttu-id="5491c-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5491c-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5491c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="5491c-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
```
# <a name="c"></a>[<span data-ttu-id="5491c-155">C#</span><span class="sxs-lookup"><span data-stu-id="5491c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5491c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5491c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5491c-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5491c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5491c-158">Java</span><span class="sxs-lookup"><span data-stu-id="5491c-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5491c-159">响应</span><span class="sxs-lookup"><span data-stu-id="5491c-159">Response</span></span>

<span data-ttu-id="5491c-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5491c-160">The following is an example of the response.</span></span>

> <span data-ttu-id="5491c-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5491c-161">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests?$skiptoken=eyJQYWdlQ29va2llIjoiPHJvdyBpZF9JZGVudGl0",
  "value": [
    {
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
    },
    {
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
    },
    {
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
    },
    {
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threatAssessmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

