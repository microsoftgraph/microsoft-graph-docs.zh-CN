---
title: 列出打印机的 printJobs
description: 检索与打印机关联的打印作业的列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 747992b4612338e6293339180868f60de3e40ebe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956288"
---
# <a name="list-printjobs-for-a-printer"></a><span data-ttu-id="29c9c-103">列出打印机的 printJobs</span><span class="sxs-lookup"><span data-stu-id="29c9c-103">List printJobs for a printer</span></span>
<span data-ttu-id="29c9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29c9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="29c9c-105">检索与打印机关联的打印作业 [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="29c9c-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29c9c-106">权限</span><span class="sxs-lookup"><span data-stu-id="29c9c-106">Permissions</span></span>
<span data-ttu-id="29c9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29c9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="29c9c-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="29c9c-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="29c9c-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="29c9c-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="29c9c-111">若要从其他用户读取打印作业，登录的用户需要是打印管理员，并且具有 PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All 或 PrintJob.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="29c9c-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="29c9c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="29c9c-112">Permission type</span></span> | <span data-ttu-id="29c9c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29c9c-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="29c9c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29c9c-114">Delegated (work or school account)</span></span>| <span data-ttu-id="29c9c-115">PrintJob.ReadBasic、PrintJob.Read、PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c9c-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="29c9c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29c9c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29c9c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="29c9c-117">Not Supported.</span></span>|
|<span data-ttu-id="29c9c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="29c9c-118">Application</span></span>| <span data-ttu-id="29c9c-119">PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c9c-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29c9c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29c9c-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29c9c-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="29c9c-121">Optional query parameters</span></span>
<span data-ttu-id="29c9c-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="29c9c-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="29c9c-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="29c9c-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="29c9c-124">默认情况下 **，响应** 中将省略 documents 属性。</span><span class="sxs-lookup"><span data-stu-id="29c9c-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="29c9c-125">若要同时返回每个 [打印作业的 printDocuments](../resources/printdocument.md) 列表，请使用 `$expand=documents` 。</span><span class="sxs-lookup"><span data-stu-id="29c9c-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="29c9c-126">此方法支持按创建打印作业的用户筛选打印作业。</span><span class="sxs-lookup"><span data-stu-id="29c9c-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="29c9c-127">使用 `$filter=createdBy/userPrincipalName eq '{upn}'` ，其中 **{upn}** 是关联 [用户](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) 的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="29c9c-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="29c9c-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="29c9c-128">Exceptions</span></span>
<span data-ttu-id="29c9c-129">不支持某些运算符 `$count` `$search` ：、。</span><span class="sxs-lookup"><span data-stu-id="29c9c-129">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29c9c-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="29c9c-130">Request headers</span></span>
|<span data-ttu-id="29c9c-131">名称</span><span class="sxs-lookup"><span data-stu-id="29c9c-131">Name</span></span>|<span data-ttu-id="29c9c-132">说明</span><span class="sxs-lookup"><span data-stu-id="29c9c-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="29c9c-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="29c9c-133">Authorization</span></span>|<span data-ttu-id="29c9c-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29c9c-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29c9c-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="29c9c-136">Request body</span></span>
<span data-ttu-id="29c9c-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29c9c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29c9c-138">响应</span><span class="sxs-lookup"><span data-stu-id="29c9c-138">Response</span></span>

<span data-ttu-id="29c9c-139">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printJob](../resources/printjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="29c9c-139">If successful, this method returns a `200 OK` response code and a collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29c9c-140">示例</span><span class="sxs-lookup"><span data-stu-id="29c9c-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29c9c-141">请求</span><span class="sxs-lookup"><span data-stu-id="29c9c-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="29c9c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="29c9c-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printjob_1"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs
```
# <a name="c"></a>[<span data-ttu-id="29c9c-143">C#</span><span class="sxs-lookup"><span data-stu-id="29c9c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printjob-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29c9c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29c9c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printjob-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29c9c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29c9c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printjob-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29c9c-146">Java</span><span class="sxs-lookup"><span data-stu-id="29c9c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printjob-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="29c9c-147">响应</span><span class="sxs-lookup"><span data-stu-id="29c9c-147">Response</span></span>
<span data-ttu-id="29c9c-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="29c9c-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('2f3453b7-4686-4b5b-9575-4f1e5b909ba7')/jobs",
  "value": [
    {
      "id": "103",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {        
      },
      "status": {
        "state": "completed",
        "description": "The print job has completed successfully and no further processing will take place.",
        "details": [          
        ],
        "isAcquiredByPrinter": true
      },
      "configuration": {        
      },
      "redirectedTo": null,
      "redirectedFrom": null,
      "isFetchable": false     
    }
  ]
}
```

