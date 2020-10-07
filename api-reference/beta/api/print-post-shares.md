---
title: 创建 printerShare
description: 为指定的打印机创建新的打印机共享。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 53752d7a6f0b703334c85582397066fa1a52f7bc
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373928"
---
# <a name="create-printershare"></a><span data-ttu-id="ff814-103">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="ff814-103">Create printerShare</span></span>

<span data-ttu-id="ff814-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff814-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff814-105">为指定的[打印机](../resources/printer.md)创建新的**printerShare** 。</span><span class="sxs-lookup"><span data-stu-id="ff814-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff814-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff814-106">Permissions</span></span>
<span data-ttu-id="ff814-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff814-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ff814-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="ff814-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="ff814-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="ff814-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ff814-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff814-111">Permission type</span></span> | <span data-ttu-id="ff814-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff814-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ff814-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff814-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ff814-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff814-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="ff814-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff814-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff814-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff814-116">Not Supported.</span></span>|
|<span data-ttu-id="ff814-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff814-117">Application</span></span>|<span data-ttu-id="ff814-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff814-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff814-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff814-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares
```
## <a name="request-headers"></a><span data-ttu-id="ff814-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff814-120">Request headers</span></span>
| <span data-ttu-id="ff814-121">名称</span><span class="sxs-lookup"><span data-stu-id="ff814-121">Name</span></span>          | <span data-ttu-id="ff814-122">说明</span><span class="sxs-lookup"><span data-stu-id="ff814-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ff814-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff814-123">Authorization</span></span> | <span data-ttu-id="ff814-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff814-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff814-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="ff814-126">Content-type</span></span>  | <span data-ttu-id="ff814-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ff814-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff814-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff814-129">Request body</span></span>
<span data-ttu-id="ff814-130">在请求正文中，提供 [printerShare](../resources/printershare.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff814-130">In the request body, supply a JSON representation of [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="ff814-131">打印机共享的 **id** 和 **createdDateTime** 属性是在创建资源时自动设置的，但共享名称和关联的打印机必须包含在请求中。</span><span class="sxs-lookup"><span data-stu-id="ff814-131">The printer share's **id** and **createdDateTime** properties are set automatically upon resource creation, but the share name and associated printer must be included in the request.</span></span>

<span data-ttu-id="ff814-132">打印机引用是使用语法设置的 `@odata.bind` ，如示例中所示。</span><span class="sxs-lookup"><span data-stu-id="ff814-132">The printer reference is set by using `@odata.bind` syntax, as shown in the example.</span></span>

## <a name="response"></a><span data-ttu-id="ff814-133">响应</span><span class="sxs-lookup"><span data-stu-id="ff814-133">Response</span></span>
<span data-ttu-id="ff814-134">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff814-134">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff814-135">示例</span><span class="sxs-lookup"><span data-stu-id="ff814-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff814-136">请求</span><span class="sxs-lookup"><span data-stu-id="ff814-136">Request</span></span>
<span data-ttu-id="ff814-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff814-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff814-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff814-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_print"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares
Content-type: application/json
Content-length: 114

{
  "name": "name-value",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="ff814-139">C#</span><span class="sxs-lookup"><span data-stu-id="ff814-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printershare-from-print-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff814-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff814-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printershare-from-print-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff814-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff814-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printershare-from-print-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ff814-142">响应</span><span class="sxs-lookup"><span data-stu-id="ff814-142">Response</span></span>
<span data-ttu-id="ff814-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff814-143">The following is an example of the response.</span></span>
><span data-ttu-id="ff814-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ff814-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 233

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
    "id": "7361c7c1-ff07-4565-9897-bef6895a7d04",
    "name": "ShareName",
    "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
