---
title: 列出 threatAssessmentRequests
description: 检索 threatassessmentrequest 对象的列表。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d81f4580072a20cfaab6e4746074ced78ebdba8f
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591584"
---
# <a name="list-threatassessmentrequests"></a><span data-ttu-id="52357-103">列出 threatAssessmentRequests</span><span class="sxs-lookup"><span data-stu-id="52357-103">List threatAssessmentRequests</span></span>

<span data-ttu-id="52357-104">检索[threatAssessmentRequest](../resources/threatassessmentrequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="52357-104">Retrieve a list of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects.</span></span>

<span data-ttu-id="52357-105">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="52357-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="52357-106">邮件</span><span class="sxs-lookup"><span data-stu-id="52357-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="52357-107">电子邮件文件</span><span class="sxs-lookup"><span data-stu-id="52357-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="52357-108">文件</span><span class="sxs-lookup"><span data-stu-id="52357-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="52357-109">URL</span><span class="sxs-lookup"><span data-stu-id="52357-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="52357-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="52357-110">Permissions</span></span>

<span data-ttu-id="52357-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52357-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="52357-113">Permission type</span></span>                        | <span data-ttu-id="52357-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52357-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52357-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52357-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="52357-116">ThreatAssessment。</span><span class="sxs-lookup"><span data-stu-id="52357-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="52357-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52357-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52357-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="52357-118">Not supported.</span></span>                              |
| <span data-ttu-id="52357-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="52357-119">Application</span></span>                            | <span data-ttu-id="52357-120">ThreatAssessment。</span><span class="sxs-lookup"><span data-stu-id="52357-120">ThreatAssessment.Read.All.</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="52357-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52357-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52357-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="52357-122">Optional query parameters</span></span>

<span data-ttu-id="52357-123">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="52357-123">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="52357-124">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="52357-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="52357-125">名称</span><span class="sxs-lookup"><span data-stu-id="52357-125">Name</span></span>            |<span data-ttu-id="52357-126">值</span><span class="sxs-lookup"><span data-stu-id="52357-126">Value</span></span>    |<span data-ttu-id="52357-127">Description</span><span class="sxs-lookup"><span data-stu-id="52357-127">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="52357-128">$filter</span><span class="sxs-lookup"><span data-stu-id="52357-128">$filter</span></span>         |<span data-ttu-id="52357-129">string</span><span class="sxs-lookup"><span data-stu-id="52357-129">string</span></span>   |<span data-ttu-id="52357-130">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="52357-130">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="52357-131">$orderby</span><span class="sxs-lookup"><span data-stu-id="52357-131">$orderby</span></span>        |<span data-ttu-id="52357-132">string</span><span class="sxs-lookup"><span data-stu-id="52357-132">string</span></span>   |<span data-ttu-id="52357-133">默认情况下，响应中的对象按其**createdDateTime**的值进行降序排序。</span><span class="sxs-lookup"><span data-stu-id="52357-133">By default, the objects in the response are descending ordered by their **createdDateTime** value.</span></span>                                                                          |
|<span data-ttu-id="52357-134">$select</span><span class="sxs-lookup"><span data-stu-id="52357-134">$select</span></span>         |<span data-ttu-id="52357-135">string</span><span class="sxs-lookup"><span data-stu-id="52357-135">string</span></span>   |<span data-ttu-id="52357-p103">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="52357-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="52357-138">$skipToken</span><span class="sxs-lookup"><span data-stu-id="52357-138">$skipToken</span></span>      |<span data-ttu-id="52357-139">string</span><span class="sxs-lookup"><span data-stu-id="52357-139">string</span></span>   |<span data-ttu-id="52357-140">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="52357-140">Retrieves the next page of results from result sets that span multiple pages.</span></span>                                                                                               |

## <a name="request-headers"></a><span data-ttu-id="52357-141">请求头</span><span class="sxs-lookup"><span data-stu-id="52357-141">Request headers</span></span>

| <span data-ttu-id="52357-142">名称</span><span class="sxs-lookup"><span data-stu-id="52357-142">Name</span></span>      |<span data-ttu-id="52357-143">说明</span><span class="sxs-lookup"><span data-stu-id="52357-143">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52357-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="52357-144">Authorization</span></span> | <span data-ttu-id="52357-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52357-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52357-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="52357-147">Request body</span></span>

<span data-ttu-id="52357-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="52357-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52357-149">响应</span><span class="sxs-lookup"><span data-stu-id="52357-149">Response</span></span>

<span data-ttu-id="52357-150">如果成功，此方法在响应`200 OK`正文中返回响应代码和[threatAssessmentRequest](../resources/threatassessmentrequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="52357-150">If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52357-151">示例</span><span class="sxs-lookup"><span data-stu-id="52357-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52357-152">请求</span><span class="sxs-lookup"><span data-stu-id="52357-152">Request</span></span>

<span data-ttu-id="52357-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="52357-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52357-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="52357-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
```

### <a name="response"></a><span data-ttu-id="52357-155">响应</span><span class="sxs-lookup"><span data-stu-id="52357-155">Response</span></span>

<span data-ttu-id="52357-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="52357-156">The following is an example of the response.</span></span>

> <span data-ttu-id="52357-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="52357-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
