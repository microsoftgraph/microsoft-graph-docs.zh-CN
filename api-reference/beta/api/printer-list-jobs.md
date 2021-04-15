---
title: 列出打印机的 printJobs
description: 检索与打印机关联的打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 190fd272fa09807ef7866bb3d34df46eb4623875
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766460"
---
# <a name="list-printjobs-for-a-printer"></a><span data-ttu-id="39e61-103">列出打印机的 printJobs</span><span class="sxs-lookup"><span data-stu-id="39e61-103">List printJobs for a printer</span></span>

<span data-ttu-id="39e61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39e61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39e61-105">检索与打印机关联的打印作业 [列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="39e61-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="39e61-106">权限</span><span class="sxs-lookup"><span data-stu-id="39e61-106">Permissions</span></span>
<span data-ttu-id="39e61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39e61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="39e61-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="39e61-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="39e61-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="39e61-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="39e61-111">若要从其他用户读取打印作业，登录的用户需要是打印管理员，并且具有 PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All 或 PrintJob.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="39e61-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="39e61-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="39e61-112">Permission type</span></span> | <span data-ttu-id="39e61-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39e61-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="39e61-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39e61-114">Delegated (work or school account)</span></span>| <span data-ttu-id="39e61-115">PrintJob.ReadBasic、PrintJob.Read、PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39e61-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="39e61-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39e61-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39e61-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="39e61-117">Not Supported.</span></span>|
|<span data-ttu-id="39e61-118">Application</span><span class="sxs-lookup"><span data-stu-id="39e61-118">Application</span></span>| <span data-ttu-id="39e61-119">PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39e61-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39e61-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39e61-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39e61-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39e61-121">Optional query parameters</span></span>
<span data-ttu-id="39e61-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="39e61-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="39e61-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="39e61-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="39e61-124">默认情况下 **，响应** 中将省略 documents 属性。</span><span class="sxs-lookup"><span data-stu-id="39e61-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="39e61-125">若要同时返回每个 [打印作业的 printDocuments](../resources/printdocument.md) 列表，请使用 `$expand=documents` 。</span><span class="sxs-lookup"><span data-stu-id="39e61-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="39e61-126">此方法支持按创建打印作业的用户筛选打印作业。</span><span class="sxs-lookup"><span data-stu-id="39e61-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="39e61-127">使用 `$filter=createdBy/userPrincipalName eq '{upn}'` ，其中 **{upn}** 是关联 [用户](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) 的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="39e61-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="39e61-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="39e61-128">Exceptions</span></span>
<span data-ttu-id="39e61-129">不支持某些运算符 `$count` `$search` ：、。</span><span class="sxs-lookup"><span data-stu-id="39e61-129">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39e61-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="39e61-130">Request headers</span></span>
| <span data-ttu-id="39e61-131">名称</span><span class="sxs-lookup"><span data-stu-id="39e61-131">Name</span></span>      |<span data-ttu-id="39e61-132">说明</span><span class="sxs-lookup"><span data-stu-id="39e61-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39e61-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="39e61-133">Authorization</span></span> | <span data-ttu-id="39e61-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39e61-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39e61-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="39e61-136">Request body</span></span>
<span data-ttu-id="39e61-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39e61-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="39e61-138">响应</span><span class="sxs-lookup"><span data-stu-id="39e61-138">Response</span></span>
<span data-ttu-id="39e61-139">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printJob](../resources/printjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="39e61-139">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39e61-140">示例</span><span class="sxs-lookup"><span data-stu-id="39e61-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="39e61-141">请求</span><span class="sxs-lookup"><span data-stu-id="39e61-141">Request</span></span>
<span data-ttu-id="39e61-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="39e61-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39e61-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="39e61-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="39e61-144">C#</span><span class="sxs-lookup"><span data-stu-id="39e61-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39e61-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39e61-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39e61-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39e61-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39e61-147">Java</span><span class="sxs-lookup"><span data-stu-id="39e61-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="39e61-148">响应</span><span class="sxs-lookup"><span data-stu-id="39e61-148">Response</span></span>
<span data-ttu-id="39e61-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="39e61-149">The following is an example of the response.</span></span>
><span data-ttu-id="39e61-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="39e61-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
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
