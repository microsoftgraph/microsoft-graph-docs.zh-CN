---
title: 为 printerShare 创建 allowedUser
description: 向指定的用户授予将打印作业提交到关联的打印机共享的权限。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ba3f98ce6059a154bc462f27c9769ac74c99be7a
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674559"
---
# <a name="create-alloweduser-for-printershare"></a><span data-ttu-id="7410c-103">为 printerShare 创建 allowedUser</span><span class="sxs-lookup"><span data-stu-id="7410c-103">Create allowedUser for printerShare</span></span>

<span data-ttu-id="7410c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7410c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7410c-105">向指定的用户授予将打印作业提交到关联的 [printerShare](../resources/printershare.md)的权限。</span><span class="sxs-lookup"><span data-stu-id="7410c-105">Grant the specified user access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7410c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7410c-106">Permissions</span></span>
<span data-ttu-id="7410c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7410c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7410c-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="7410c-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="7410c-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="7410c-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="7410c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7410c-111">Permission type</span></span> | <span data-ttu-id="7410c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7410c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7410c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7410c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7410c-114">PrinterShare</span><span class="sxs-lookup"><span data-stu-id="7410c-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="7410c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7410c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7410c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7410c-116">Not Supported.</span></span>|
|<span data-ttu-id="7410c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7410c-117">Application</span></span>|<span data-ttu-id="7410c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7410c-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7410c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7410c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedUsers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7410c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7410c-120">Request headers</span></span>
| <span data-ttu-id="7410c-121">名称</span><span class="sxs-lookup"><span data-stu-id="7410c-121">Name</span></span>          | <span data-ttu-id="7410c-122">说明</span><span class="sxs-lookup"><span data-stu-id="7410c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7410c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7410c-123">Authorization</span></span> | <span data-ttu-id="7410c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7410c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7410c-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="7410c-126">Content-type</span></span>  | <span data-ttu-id="7410c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7410c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7410c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7410c-129">Request body</span></span>
<span data-ttu-id="7410c-130">在请求正文中，通过使用格式提供对用户实体的引用 `@odata.id` ，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="7410c-130">In the request body, supply a reference to a user entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="7410c-131">响应</span><span class="sxs-lookup"><span data-stu-id="7410c-131">Response</span></span>
<span data-ttu-id="7410c-132">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7410c-132">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7410c-133">示例</span><span class="sxs-lookup"><span data-stu-id="7410c-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7410c-134">请求</span><span class="sxs-lookup"><span data-stu-id="7410c-134">Request</span></span>
<span data-ttu-id="7410c-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7410c-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7410c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7410c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_alloweduser_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/{id}/allowedUsers/$ref
Content-type: application/json
Content-length: 66

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="7410c-137">C#</span><span class="sxs-lookup"><span data-stu-id="7410c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-alloweduser-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7410c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7410c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-alloweduser-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7410c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7410c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-alloweduser-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7410c-140">在请求正文中，通过在 JSON 正文的字段中添加用户的 Microsoft Graph URI，提供对用户实体的引用 `@odata.id` 。</span><span class="sxs-lookup"><span data-stu-id="7410c-140">In the request body, supply a reference to a user entity by including the user's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="7410c-141">响应</span><span class="sxs-lookup"><span data-stu-id="7410c-141">Response</span></span>
<span data-ttu-id="7410c-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7410c-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
