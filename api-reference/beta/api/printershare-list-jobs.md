---
title: 列出 printerShare 的 printJobs
description: 检索与打印共享关联的打印作业列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7453677550e974536de20b6ad2b054d2040990e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037455"
---
# <a name="list-printjobs-for-a-printershare"></a><span data-ttu-id="92d12-103">列出 printerShare 的 printJobs</span><span class="sxs-lookup"><span data-stu-id="92d12-103">List printJobs for a printerShare</span></span>

<span data-ttu-id="92d12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92d12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92d12-105">检索与 [printerShare](../resources/printershare.md)关联的打印作业列表。</span><span class="sxs-lookup"><span data-stu-id="92d12-105">Retrieve a list of print jobs associated with the [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="92d12-106">权限</span><span class="sxs-lookup"><span data-stu-id="92d12-106">Permissions</span></span>
<span data-ttu-id="92d12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="92d12-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予 [获取 printerShare](printershare-get.md) 访问权限的权限以及下表中列出的权限之一。</span><span class="sxs-lookup"><span data-stu-id="92d12-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printerShare](printershare-get.md) access, and one of the permissions listed in the following table.</span></span> 

<span data-ttu-id="92d12-110">若要从其他用户读取打印作业，登录的用户需要是打印管理员，并且具有 PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All 或 PrintJob.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="92d12-110">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="92d12-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="92d12-111">Permission type</span></span> | <span data-ttu-id="92d12-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92d12-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="92d12-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92d12-113">Delegated (work or school account)</span></span>| <span data-ttu-id="92d12-114">PrintJob.ReadBasic、PrintJob.Read、PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d12-114">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="92d12-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92d12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92d12-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="92d12-116">Not Supported.</span></span>|
|<span data-ttu-id="92d12-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="92d12-117">Application</span></span>| <span data-ttu-id="92d12-118">PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d12-118">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92d12-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92d12-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92d12-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="92d12-120">Optional query parameters</span></span>
<span data-ttu-id="92d12-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="92d12-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="92d12-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="92d12-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="92d12-123">默认情况下 **，响应** 中将省略 documents 属性。</span><span class="sxs-lookup"><span data-stu-id="92d12-123">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="92d12-124">若要同时返回每个 [打印作业的 printDocuments](../resources/printdocument.md) 列表，请使用 `$expand=documents` 。</span><span class="sxs-lookup"><span data-stu-id="92d12-124">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="92d12-125">此方法支持按创建打印作业的用户筛选打印作业。</span><span class="sxs-lookup"><span data-stu-id="92d12-125">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="92d12-126">使用 `$filter=createdBy/userPrincipalName eq '{upn}'` ，其中 **{upn}** 是关联 [用户](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) 的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="92d12-126">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="92d12-127">Exceptions</span><span class="sxs-lookup"><span data-stu-id="92d12-127">Exceptions</span></span>
<span data-ttu-id="92d12-128">不支持某些运算符 `$count` `$search` ：、。</span><span class="sxs-lookup"><span data-stu-id="92d12-128">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92d12-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="92d12-129">Request headers</span></span>
| <span data-ttu-id="92d12-130">名称</span><span class="sxs-lookup"><span data-stu-id="92d12-130">Name</span></span>      |<span data-ttu-id="92d12-131">说明</span><span class="sxs-lookup"><span data-stu-id="92d12-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92d12-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="92d12-132">Authorization</span></span> | <span data-ttu-id="92d12-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92d12-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92d12-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="92d12-135">Request body</span></span>
<span data-ttu-id="92d12-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92d12-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="92d12-137">响应</span><span class="sxs-lookup"><span data-stu-id="92d12-137">Response</span></span>
<span data-ttu-id="92d12-138">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printJob](../resources/printjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="92d12-138">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92d12-139">示例</span><span class="sxs-lookup"><span data-stu-id="92d12-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="92d12-140">请求</span><span class="sxs-lookup"><span data-stu-id="92d12-140">Request</span></span>
<span data-ttu-id="92d12-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92d12-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92d12-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="92d12-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="92d12-143">C#</span><span class="sxs-lookup"><span data-stu-id="92d12-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92d12-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92d12-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92d12-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92d12-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92d12-146">Java</span><span class="sxs-lookup"><span data-stu-id="92d12-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="92d12-147">响应</span><span class="sxs-lookup"><span data-stu-id="92d12-147">Response</span></span>
<span data-ttu-id="92d12-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92d12-148">The following is an example of the response.</span></span>
><span data-ttu-id="92d12-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="92d12-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares('f37141d9-0afb-484f-96d3-0ef0a679e6c1')/jobs",
  "value": [
    {
      "id": "103",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "state": "completed",
        "description": "The print job has completed successfully and no further processing will take place.",
        "details" : [],
        "isAcquiredByPrinter": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
