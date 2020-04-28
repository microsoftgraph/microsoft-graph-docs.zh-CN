---
title: 列出 allowedGroups
description: 检索已授予访问权限的组列表，以将打印作业提交到关联的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d3c9535f3a9ecf1e70e96eb564d2a7249b9fd130
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917010"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="d5a08-103">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="d5a08-103">List allowedGroups</span></span>

<span data-ttu-id="d5a08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5a08-105">检索已授予访问权限的组列表，以将打印作业提交到关联的[打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="d5a08-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5a08-106">权限</span><span class="sxs-lookup"><span data-stu-id="d5a08-106">Permissions</span></span>
<span data-ttu-id="d5a08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5a08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d5a08-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="d5a08-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d5a08-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5a08-110">Permission type</span></span> | <span data-ttu-id="d5a08-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5a08-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d5a08-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5a08-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d5a08-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="d5a08-113">Users.Read.All</span></span> |
|<span data-ttu-id="d5a08-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5a08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5a08-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5a08-115">Not Supported.</span></span>|
|<span data-ttu-id="d5a08-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5a08-116">Application</span></span>|<span data-ttu-id="d5a08-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5a08-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5a08-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5a08-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5a08-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d5a08-119">Optional query parameters</span></span>
<span data-ttu-id="d5a08-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5a08-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d5a08-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d5a08-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5a08-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5a08-122">Request headers</span></span>
| <span data-ttu-id="d5a08-123">名称</span><span class="sxs-lookup"><span data-stu-id="d5a08-123">Name</span></span>      |<span data-ttu-id="d5a08-124">说明</span><span class="sxs-lookup"><span data-stu-id="d5a08-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5a08-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5a08-125">Authorization</span></span> | <span data-ttu-id="d5a08-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5a08-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5a08-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5a08-128">Request body</span></span>
<span data-ttu-id="d5a08-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5a08-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d5a08-130">响应</span><span class="sxs-lookup"><span data-stu-id="d5a08-130">Response</span></span>
<span data-ttu-id="d5a08-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printIdentity](../resources/printidentity.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d5a08-131">If successful, this method returns a `200 OK` response code and a collection of [printIdentity](../resources/printidentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5a08-132">示例</span><span class="sxs-lookup"><span data-stu-id="d5a08-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5a08-133">请求</span><span class="sxs-lookup"><span data-stu-id="d5a08-133">Request</span></span>
<span data-ttu-id="d5a08-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d5a08-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5a08-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5a08-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="d5a08-136">C#</span><span class="sxs-lookup"><span data-stu-id="d5a08-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5a08-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5a08-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5a08-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5a08-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d5a08-139">响应</span><span class="sxs-lookup"><span data-stu-id="d5a08-139">Response</span></span>
<span data-ttu-id="d5a08-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d5a08-140">The following is an example of the response.</span></span>
><span data-ttu-id="d5a08-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d5a08-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printIdentity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "GroupName"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
