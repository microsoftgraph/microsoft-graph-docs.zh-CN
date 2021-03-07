---
title: 列出 printerShare 的 printJobs
description: 检索与打印共享关联的打印作业列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9979870573e84d10c552e70205fab2494e289fc7
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516985"
---
# <a name="list-printjobs-for-a-printershare"></a><span data-ttu-id="be9b3-103">列出 printerShare 的 printJobs</span><span class="sxs-lookup"><span data-stu-id="be9b3-103">List printJobs for a printerShare</span></span>
<span data-ttu-id="be9b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be9b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="be9b3-105">检索与 printerShare 关联的打印 [作业列表](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="be9b3-105">Retrieve a list of print jobs associated with the [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be9b3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="be9b3-106">Permissions</span></span>
<span data-ttu-id="be9b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be9b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="be9b3-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予 [获取 printerShare](printershare-get.md) 访问权限的权限以及下表中列出的权限之一。</span><span class="sxs-lookup"><span data-stu-id="be9b3-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printerShare](printershare-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="be9b3-110">登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="be9b3-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="be9b3-111">若要从其他用户读取打印作业，登录用户需要是打印管理员，并且具有 PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All 或 PrintJob.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="be9b3-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="be9b3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="be9b3-112">Permission type</span></span> | <span data-ttu-id="be9b3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be9b3-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="be9b3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be9b3-114">Delegated (work or school account)</span></span>| <span data-ttu-id="be9b3-115">PrintJob.ReadBasic、PrintJob.Read、PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9b3-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="be9b3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be9b3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be9b3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="be9b3-117">Not Supported.</span></span>|
|<span data-ttu-id="be9b3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="be9b3-118">Application</span></span>| <span data-ttu-id="be9b3-119">PrintJob.ReadBasic.All、PrintJob.Read.All、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9b3-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be9b3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be9b3-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be9b3-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be9b3-121">Optional query parameters</span></span>
<span data-ttu-id="be9b3-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be9b3-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="be9b3-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="be9b3-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="be9b3-124">默认情况下 **，响应** 中将省略 documents 属性。</span><span class="sxs-lookup"><span data-stu-id="be9b3-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="be9b3-125">若要同时返回每个打印作业 [的 printDocuments](../resources/printdocument.md) 列表，请使用 `$expand=documents` 。</span><span class="sxs-lookup"><span data-stu-id="be9b3-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="be9b3-126">此方法支持按创建作业的用户筛选打印作业。</span><span class="sxs-lookup"><span data-stu-id="be9b3-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="be9b3-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'` ，其中 **{upn}** 是关联用户的用户主体名称。 [](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname)</span><span class="sxs-lookup"><span data-stu-id="be9b3-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="be9b3-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="be9b3-128">Exceptions</span></span>
<span data-ttu-id="be9b3-129">不支持某些运算符： `$count` `$search` .</span><span class="sxs-lookup"><span data-stu-id="be9b3-129">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be9b3-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="be9b3-130">Request headers</span></span>
|<span data-ttu-id="be9b3-131">名称</span><span class="sxs-lookup"><span data-stu-id="be9b3-131">Name</span></span>|<span data-ttu-id="be9b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="be9b3-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="be9b3-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="be9b3-133">Authorization</span></span>|<span data-ttu-id="be9b3-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be9b3-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be9b3-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="be9b3-136">Request body</span></span>
<span data-ttu-id="be9b3-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be9b3-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be9b3-138">响应</span><span class="sxs-lookup"><span data-stu-id="be9b3-138">Response</span></span>

<span data-ttu-id="be9b3-139">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printJob](../resources/printjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="be9b3-139">If successful, this method returns a `200 OK` response code and a collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be9b3-140">示例</span><span class="sxs-lookup"><span data-stu-id="be9b3-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be9b3-141">请求</span><span class="sxs-lookup"><span data-stu-id="be9b3-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printjob"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs
```

### <a name="response"></a><span data-ttu-id="be9b3-142">响应</span><span class="sxs-lookup"><span data-stu-id="be9b3-142">Response</span></span>
<span data-ttu-id="be9b3-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="be9b3-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares('f37141d9-0afb-484f-96d3-0ef0a679e6c1')/jobs",
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

