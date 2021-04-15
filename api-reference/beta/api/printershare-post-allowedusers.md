---
title: 为 printerShare 创建 allowedUser
description: 向指定的用户授予将打印作业提交到关联的打印机共享的权限。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c3c170c05d8dfe18a228456de26c3bbce4dabc2a
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765941"
---
# <a name="create-alloweduser-for-printershare"></a><span data-ttu-id="bf729-103">为 printerShare 创建 allowedUser</span><span class="sxs-lookup"><span data-stu-id="bf729-103">Create allowedUser for printerShare</span></span>

<span data-ttu-id="bf729-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf729-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf729-105">授予指定用户向关联的 printerShare 提交打印 [作业的权限](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="bf729-105">Grant the specified user access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf729-106">权限</span><span class="sxs-lookup"><span data-stu-id="bf729-106">Permissions</span></span>
<span data-ttu-id="bf729-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bf729-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="bf729-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="bf729-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="bf729-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="bf729-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf729-111">Permission type</span></span> | <span data-ttu-id="bf729-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf729-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bf729-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf729-113">Delegated (work or school account)</span></span>| <span data-ttu-id="bf729-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf729-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="bf729-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf729-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf729-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf729-116">Not Supported.</span></span>|
|<span data-ttu-id="bf729-117">Application</span><span class="sxs-lookup"><span data-stu-id="bf729-117">Application</span></span>|<span data-ttu-id="bf729-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf729-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf729-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf729-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/allowedUsers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bf729-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf729-120">Request headers</span></span>
| <span data-ttu-id="bf729-121">名称</span><span class="sxs-lookup"><span data-stu-id="bf729-121">Name</span></span>          | <span data-ttu-id="bf729-122">说明</span><span class="sxs-lookup"><span data-stu-id="bf729-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bf729-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf729-123">Authorization</span></span> | <span data-ttu-id="bf729-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf729-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf729-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="bf729-126">Content-type</span></span>  | <span data-ttu-id="bf729-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bf729-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf729-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf729-129">Request body</span></span>
<span data-ttu-id="bf729-130">在请求正文中，使用 格式提供对用户实体的引用， `@odata.id` 如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="bf729-130">In the request body, supply a reference to a user entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="bf729-131">响应</span><span class="sxs-lookup"><span data-stu-id="bf729-131">Response</span></span>
<span data-ttu-id="bf729-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bf729-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bf729-133">示例</span><span class="sxs-lookup"><span data-stu-id="bf729-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf729-134">请求</span><span class="sxs-lookup"><span data-stu-id="bf729-134">Request</span></span>
<span data-ttu-id="bf729-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bf729-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bf729-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf729-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bf729-137">C#</span><span class="sxs-lookup"><span data-stu-id="bf729-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-alloweduser-from-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf729-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf729-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-alloweduser-from-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf729-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf729-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-alloweduser-from-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf729-140">Java</span><span class="sxs-lookup"><span data-stu-id="bf729-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-alloweduser-from-printers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bf729-141">在请求正文中，提供对用户实体的引用，将用户的 Microsoft Graph URI 包括在 JSON 正文的 `@odata.id` 字段中。</span><span class="sxs-lookup"><span data-stu-id="bf729-141">In the request body, supply a reference to a user entity by including the user's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="bf729-142">响应</span><span class="sxs-lookup"><span data-stu-id="bf729-142">Response</span></span>
<span data-ttu-id="bf729-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bf729-143">The following is an example of the response.</span></span> 
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
