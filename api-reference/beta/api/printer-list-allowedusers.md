---
title: 列出打印机的 allowedUsers
description: 检索已授予访问权限以将打印作业提交到关联打印机的用户的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: fe7aaadc66281d85dd3930677ca81dbad18163bd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035734"
---
# <a name="list-allowedusers-for-printer"></a><span data-ttu-id="682d0-103">列出打印机的 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="682d0-103">List allowedUsers for printer</span></span>

<span data-ttu-id="682d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="682d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="682d0-105">检索已授予访问权限以将打印作业提交到关联 [打印机](../resources/printer.md)的用户的列表。</span><span class="sxs-lookup"><span data-stu-id="682d0-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="682d0-106">权限</span><span class="sxs-lookup"><span data-stu-id="682d0-106">Permissions</span></span>
<span data-ttu-id="682d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="682d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="682d0-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="682d0-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="682d0-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="682d0-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="682d0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="682d0-111">Permission type</span></span> | <span data-ttu-id="682d0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="682d0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="682d0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="682d0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="682d0-114">Printer。 all，完全控制，All，All</span><span class="sxs-lookup"><span data-stu-id="682d0-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="682d0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="682d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="682d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="682d0-116">Not Supported.</span></span>|
|<span data-ttu-id="682d0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="682d0-117">Application</span></span>| <span data-ttu-id="682d0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="682d0-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="682d0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="682d0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="682d0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="682d0-120">Optional query parameters</span></span>
<span data-ttu-id="682d0-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="682d0-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="682d0-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="682d0-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="682d0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="682d0-123">Request headers</span></span>
| <span data-ttu-id="682d0-124">名称</span><span class="sxs-lookup"><span data-stu-id="682d0-124">Name</span></span>      |<span data-ttu-id="682d0-125">说明</span><span class="sxs-lookup"><span data-stu-id="682d0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="682d0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="682d0-126">Authorization</span></span> | <span data-ttu-id="682d0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="682d0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="682d0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="682d0-129">Request body</span></span>
<span data-ttu-id="682d0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="682d0-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="682d0-131">响应</span><span class="sxs-lookup"><span data-stu-id="682d0-131">Response</span></span>
<span data-ttu-id="682d0-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printUserIdentity](../resources/printuseridentity.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="682d0-132">If successful, this method returns a `200 OK` response code and a collection of [printUserIdentity](../resources/printuseridentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="682d0-133">示例</span><span class="sxs-lookup"><span data-stu-id="682d0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="682d0-134">请求</span><span class="sxs-lookup"><span data-stu-id="682d0-134">Request</span></span>
<span data-ttu-id="682d0-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="682d0-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="682d0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="682d0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="682d0-137">C#</span><span class="sxs-lookup"><span data-stu-id="682d0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="682d0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="682d0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="682d0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="682d0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="682d0-140">响应</span><span class="sxs-lookup"><span data-stu-id="682d0-140">Response</span></span>
<span data-ttu-id="682d0-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="682d0-141">The following is an example of the response.</span></span>
><span data-ttu-id="682d0-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="682d0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUserIdentity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 286

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printUserIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


