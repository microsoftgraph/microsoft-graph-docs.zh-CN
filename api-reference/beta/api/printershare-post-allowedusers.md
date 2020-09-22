---
title: 为 printerShare 创建 allowedUser
description: 向指定的用户授予将打印作业提交到关联的打印机共享的权限。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7304f4b47e06e650d7bba4bc2ad58face6299370
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035481"
---
# <a name="create-alloweduser-for-printershare"></a><span data-ttu-id="c10e8-103">为 printerShare 创建 allowedUser</span><span class="sxs-lookup"><span data-stu-id="c10e8-103">Create allowedUser for printerShare</span></span>

<span data-ttu-id="c10e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c10e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c10e8-105">向指定的用户授予将打印作业提交到关联的 [printerShare](../resources/printershare.md)的权限。</span><span class="sxs-lookup"><span data-stu-id="c10e8-105">Grant the specified user access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c10e8-106">权限</span><span class="sxs-lookup"><span data-stu-id="c10e8-106">Permissions</span></span>
<span data-ttu-id="c10e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c10e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c10e8-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="c10e8-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c10e8-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="c10e8-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c10e8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c10e8-111">Permission type</span></span> | <span data-ttu-id="c10e8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c10e8-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c10e8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c10e8-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c10e8-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c10e8-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="c10e8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c10e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c10e8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c10e8-116">Not Supported.</span></span>|
|<span data-ttu-id="c10e8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c10e8-117">Application</span></span>|<span data-ttu-id="c10e8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c10e8-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c10e8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c10e8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedUsers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c10e8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c10e8-120">Request headers</span></span>
| <span data-ttu-id="c10e8-121">名称</span><span class="sxs-lookup"><span data-stu-id="c10e8-121">Name</span></span>          | <span data-ttu-id="c10e8-122">说明</span><span class="sxs-lookup"><span data-stu-id="c10e8-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c10e8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c10e8-123">Authorization</span></span> | <span data-ttu-id="c10e8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c10e8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c10e8-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c10e8-126">Content-type</span></span>  | <span data-ttu-id="c10e8-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c10e8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c10e8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c10e8-129">Request body</span></span>
<span data-ttu-id="c10e8-130">在请求正文中，通过使用格式提供对用户实体的引用 `@odata.id` ，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="c10e8-130">In the request body, supply a reference to a user entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="c10e8-131">响应</span><span class="sxs-lookup"><span data-stu-id="c10e8-131">Response</span></span>
<span data-ttu-id="c10e8-132">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c10e8-132">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c10e8-133">示例</span><span class="sxs-lookup"><span data-stu-id="c10e8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c10e8-134">请求</span><span class="sxs-lookup"><span data-stu-id="c10e8-134">Request</span></span>
<span data-ttu-id="c10e8-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c10e8-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c10e8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c10e8-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c10e8-137">C#</span><span class="sxs-lookup"><span data-stu-id="c10e8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-alloweduser-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c10e8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c10e8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-alloweduser-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c10e8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c10e8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-alloweduser-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c10e8-140">在请求正文中，通过在 JSON 正文的字段中添加用户的 Microsoft Graph URI，提供对用户实体的引用 `@odata.id` 。</span><span class="sxs-lookup"><span data-stu-id="c10e8-140">In the request body, supply a reference to a user entity by including the user's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="c10e8-141">响应</span><span class="sxs-lookup"><span data-stu-id="c10e8-141">Response</span></span>
<span data-ttu-id="c10e8-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c10e8-142">The following is an example of the response.</span></span> 
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


