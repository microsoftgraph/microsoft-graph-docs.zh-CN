---
title: 列出 printerShare 的 allowedUsers
description: 检索已被授予将打印作业提交到关联的打印机共享的权限的用户的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d66ba6d7d9eadecc4b6b1dc2346fbf6afe1e7378
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766005"
---
# <a name="list-allowedusers-for-printershare"></a><span data-ttu-id="685b5-103">列出 printerShare 的 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="685b5-103">List allowedUsers for printerShare</span></span>

<span data-ttu-id="685b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="685b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="685b5-105">检索已被授予向关联的 printerShare 提交打印作业的权限 [的用户列表](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="685b5-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="685b5-106">权限</span><span class="sxs-lookup"><span data-stu-id="685b5-106">Permissions</span></span>
<span data-ttu-id="685b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="685b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="685b5-109">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [列表用户访问权限](user-list.md) 的权限。</span><span class="sxs-lookup"><span data-stu-id="685b5-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List users](user-list.md) access.</span></span> <span data-ttu-id="685b5-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="685b5-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="685b5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="685b5-111">Permission type</span></span> | <span data-ttu-id="685b5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="685b5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="685b5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="685b5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="685b5-114">PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="685b5-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="685b5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="685b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="685b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="685b5-116">Not Supported.</span></span>|
|<span data-ttu-id="685b5-117">Application</span><span class="sxs-lookup"><span data-stu-id="685b5-117">Application</span></span>|<span data-ttu-id="685b5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="685b5-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="685b5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="685b5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="685b5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="685b5-120">Request headers</span></span>
| <span data-ttu-id="685b5-121">名称</span><span class="sxs-lookup"><span data-stu-id="685b5-121">Name</span></span>      |<span data-ttu-id="685b5-122">说明</span><span class="sxs-lookup"><span data-stu-id="685b5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="685b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="685b5-123">Authorization</span></span> | <span data-ttu-id="685b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="685b5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="685b5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="685b5-126">Request body</span></span>
<span data-ttu-id="685b5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="685b5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="685b5-128">响应</span><span class="sxs-lookup"><span data-stu-id="685b5-128">Response</span></span>
<span data-ttu-id="685b5-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="685b5-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="685b5-130">示例</span><span class="sxs-lookup"><span data-stu-id="685b5-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="685b5-131">请求</span><span class="sxs-lookup"><span data-stu-id="685b5-131">Request</span></span>
<span data-ttu-id="685b5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="685b5-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="685b5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="685b5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="685b5-134">C#</span><span class="sxs-lookup"><span data-stu-id="685b5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="685b5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="685b5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="685b5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="685b5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="685b5-137">Java</span><span class="sxs-lookup"><span data-stu-id="685b5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allowedusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="685b5-138">响应</span><span class="sxs-lookup"><span data-stu-id="685b5-138">Response</span></span>
<span data-ttu-id="685b5-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="685b5-139">The following is an example of the response.</span></span>
><span data-ttu-id="685b5-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="685b5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 286

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.user)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@contoso.com"
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
