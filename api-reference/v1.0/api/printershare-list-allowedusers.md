---
title: 列出 printerShare 的 allowedUsers
description: 检索已被授予将打印作业提交到关联的打印机共享的权限的用户的列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d1f55d9d4ae91d6ae41ee4656fbb1e90b7948304
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771531"
---
# <a name="list-allowedusers"></a><span data-ttu-id="dc1a9-103">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="dc1a9-103">List allowedUsers</span></span>
<span data-ttu-id="dc1a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc1a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="dc1a9-105">检索已被授予向关联的 printerShare 提交打印作业的权限 [的用户列表](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc1a9-106">权限</span><span class="sxs-lookup"><span data-stu-id="dc1a9-106">Permissions</span></span>
<span data-ttu-id="dc1a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dc1a9-109">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [列表用户访问权限](user-list.md) 的权限。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List users](user-list.md) access.</span></span> <span data-ttu-id="dc1a9-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="dc1a9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc1a9-111">Permission type</span></span> | <span data-ttu-id="dc1a9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc1a9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="dc1a9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc1a9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="dc1a9-114">PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc1a9-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="dc1a9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc1a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc1a9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-116">Not Supported.</span></span>|
|<span data-ttu-id="dc1a9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc1a9-117">Application</span></span>|<span data-ttu-id="dc1a9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc1a9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc1a9-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="dc1a9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc1a9-120">Request headers</span></span>
|<span data-ttu-id="dc1a9-121">名称</span><span class="sxs-lookup"><span data-stu-id="dc1a9-121">Name</span></span>|<span data-ttu-id="dc1a9-122">说明</span><span class="sxs-lookup"><span data-stu-id="dc1a9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc1a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc1a9-123">Authorization</span></span>|<span data-ttu-id="dc1a9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc1a9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc1a9-126">Request body</span></span>
<span data-ttu-id="dc1a9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc1a9-128">响应</span><span class="sxs-lookup"><span data-stu-id="dc1a9-128">Response</span></span>

<span data-ttu-id="dc1a9-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc1a9-130">示例</span><span class="sxs-lookup"><span data-stu-id="dc1a9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc1a9-131">请求</span><span class="sxs-lookup"><span data-stu-id="dc1a9-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dc1a9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc1a9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_user"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="dc1a9-133">C#</span><span class="sxs-lookup"><span data-stu-id="dc1a9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc1a9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc1a9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc1a9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc1a9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc1a9-136">Java</span><span class="sxs-lookup"><span data-stu-id="dc1a9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dc1a9-137">响应</span><span class="sxs-lookup"><span data-stu-id="dc1a9-137">Response</span></span>
<span data-ttu-id="dc1a9-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dc1a9-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.user)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.user)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@contoso.com"
    }
  ]
}
```

