---
title: 列出 threatAssessmentRequests
description: 检索 threatassessmentrequest 对象的列表。
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d830c80c71e0873806d67ff0e6196a1bdc4d6483
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040509"
---
# <a name="list-threatassessmentrequests"></a><span data-ttu-id="256d2-103">列出 threatAssessmentRequests</span><span class="sxs-lookup"><span data-stu-id="256d2-103">List threatAssessmentRequests</span></span>

<span data-ttu-id="256d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="256d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="256d2-105">检索 [threatAssessmentRequest 对象](../resources/threatassessmentrequest.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="256d2-105">Retrieve a list of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects.</span></span>

<span data-ttu-id="256d2-106">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="256d2-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="256d2-107">邮件</span><span class="sxs-lookup"><span data-stu-id="256d2-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="256d2-108">电子邮件文件</span><span class="sxs-lookup"><span data-stu-id="256d2-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="256d2-109">文件</span><span class="sxs-lookup"><span data-stu-id="256d2-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="256d2-110">URL</span><span class="sxs-lookup"><span data-stu-id="256d2-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="256d2-111">权限</span><span class="sxs-lookup"><span data-stu-id="256d2-111">Permissions</span></span>

<span data-ttu-id="256d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="256d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="256d2-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="256d2-114">Permission type</span></span>                        | <span data-ttu-id="256d2-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="256d2-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="256d2-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="256d2-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="256d2-117">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256d2-117">ThreatAssessment.ReadWrite.All</span></span>             |
| <span data-ttu-id="256d2-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="256d2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="256d2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="256d2-119">Not supported.</span></span>                              |
| <span data-ttu-id="256d2-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="256d2-120">Application</span></span>                            | <span data-ttu-id="256d2-121">ThreatAssessment.Read.All</span><span class="sxs-lookup"><span data-stu-id="256d2-121">ThreatAssessment.Read.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="256d2-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="256d2-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="256d2-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="256d2-123">Optional query parameters</span></span>

<span data-ttu-id="256d2-124">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="256d2-124">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="256d2-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="256d2-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="256d2-126">名称</span><span class="sxs-lookup"><span data-stu-id="256d2-126">Name</span></span>            |<span data-ttu-id="256d2-127">值</span><span class="sxs-lookup"><span data-stu-id="256d2-127">Value</span></span>    |<span data-ttu-id="256d2-128">说明</span><span class="sxs-lookup"><span data-stu-id="256d2-128">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="256d2-129">$filter</span><span class="sxs-lookup"><span data-stu-id="256d2-129">$filter</span></span>         |<span data-ttu-id="256d2-130">string</span><span class="sxs-lookup"><span data-stu-id="256d2-130">string</span></span>   |<span data-ttu-id="256d2-131">将响应限制到仅包含指定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="256d2-131">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="256d2-132">$orderby</span><span class="sxs-lookup"><span data-stu-id="256d2-132">$orderby</span></span>        |<span data-ttu-id="256d2-133">string</span><span class="sxs-lookup"><span data-stu-id="256d2-133">string</span></span>   |<span data-ttu-id="256d2-134">默认情况下，响应中的对象按 **其 createdDateTime** 值降序排序。</span><span class="sxs-lookup"><span data-stu-id="256d2-134">By default, the objects in the response are descending ordered by their **createdDateTime** value.</span></span>                                                                          |
|<span data-ttu-id="256d2-135">$select</span><span class="sxs-lookup"><span data-stu-id="256d2-135">$select</span></span>         |<span data-ttu-id="256d2-136">string</span><span class="sxs-lookup"><span data-stu-id="256d2-136">string</span></span>   |<span data-ttu-id="256d2-p103">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="256d2-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="256d2-139">$skipToken</span><span class="sxs-lookup"><span data-stu-id="256d2-139">$skipToken</span></span>      |<span data-ttu-id="256d2-140">string</span><span class="sxs-lookup"><span data-stu-id="256d2-140">string</span></span>   |<span data-ttu-id="256d2-141">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="256d2-141">Retrieves the next page of results from result sets that span multiple pages.</span></span>                                                                                               |

## <a name="request-headers"></a><span data-ttu-id="256d2-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="256d2-142">Request headers</span></span>

| <span data-ttu-id="256d2-143">名称</span><span class="sxs-lookup"><span data-stu-id="256d2-143">Name</span></span>      |<span data-ttu-id="256d2-144">说明</span><span class="sxs-lookup"><span data-stu-id="256d2-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="256d2-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="256d2-145">Authorization</span></span> | <span data-ttu-id="256d2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="256d2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="256d2-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="256d2-148">Request body</span></span>

<span data-ttu-id="256d2-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="256d2-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="256d2-150">响应</span><span class="sxs-lookup"><span data-stu-id="256d2-150">Response</span></span>

<span data-ttu-id="256d2-151">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [threatAssessmentRequest](../resources/threatassessmentrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="256d2-151">If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="256d2-152">示例</span><span class="sxs-lookup"><span data-stu-id="256d2-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="256d2-153">请求</span><span class="sxs-lookup"><span data-stu-id="256d2-153">Request</span></span>

<span data-ttu-id="256d2-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="256d2-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="256d2-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="256d2-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
```
# <a name="c"></a>[<span data-ttu-id="256d2-156">C#</span><span class="sxs-lookup"><span data-stu-id="256d2-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="256d2-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="256d2-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="256d2-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="256d2-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="256d2-159">Java</span><span class="sxs-lookup"><span data-stu-id="256d2-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="256d2-160">响应</span><span class="sxs-lookup"><span data-stu-id="256d2-160">Response</span></span>

<span data-ttu-id="256d2-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="256d2-161">The following is an example of the response.</span></span>

> <span data-ttu-id="256d2-162">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="256d2-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests",
  "@odata.nextLink": "https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests?$skiptoken=eyJQYWdlQ29va2llIjoiPHJvdyBpZF9JZGVudGl0",
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
      "messageUri": "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
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


