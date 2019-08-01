---
title: 'mailFolder: copy'
description: 将 mailfolder 及其内容复制到其他 mailfolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 277d058788efef9ec3ecf9ecb1ea21ab74ccd8c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023113"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="809f7-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="809f7-103">mailFolder: copy</span></span>

<span data-ttu-id="809f7-104">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="809f7-104">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="809f7-105">权限</span><span class="sxs-lookup"><span data-stu-id="809f7-105">Permissions</span></span>

<span data-ttu-id="809f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="809f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="809f7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="809f7-108">Permission type</span></span> | <span data-ttu-id="809f7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="809f7-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="809f7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="809f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="809f7-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="809f7-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="809f7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="809f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="809f7-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="809f7-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="809f7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="809f7-114">Application</span></span> | <span data-ttu-id="809f7-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="809f7-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="809f7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="809f7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="809f7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="809f7-117">Request headers</span></span>
| <span data-ttu-id="809f7-118">标头</span><span class="sxs-lookup"><span data-stu-id="809f7-118">Header</span></span> | <span data-ttu-id="809f7-119">值</span><span class="sxs-lookup"><span data-stu-id="809f7-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="809f7-120">授权</span><span class="sxs-lookup"><span data-stu-id="809f7-120">Authorization</span></span> | <span data-ttu-id="809f7-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="809f7-121"></span></span> <span data-ttu-id="809f7-122">必需。</span><span class="sxs-lookup"><span data-stu-id="809f7-122">Required.</span></span> |
| <span data-ttu-id="809f7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="809f7-123">Content-Type</span></span> | <span data-ttu-id="809f7-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="809f7-124"></span></span> <span data-ttu-id="809f7-125">必需。</span><span class="sxs-lookup"><span data-stu-id="809f7-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="809f7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="809f7-126">Request body</span></span>

<span data-ttu-id="809f7-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="809f7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="809f7-128">参数</span><span class="sxs-lookup"><span data-stu-id="809f7-128">Parameter</span></span> | <span data-ttu-id="809f7-129">类型</span><span class="sxs-lookup"><span data-stu-id="809f7-129">Type</span></span> | <span data-ttu-id="809f7-130">说明</span><span class="sxs-lookup"><span data-stu-id="809f7-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="809f7-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="809f7-131">destinationId</span></span>|<span data-ttu-id="809f7-132">String</span><span class="sxs-lookup"><span data-stu-id="809f7-132">String</span></span>|<span data-ttu-id="809f7-133">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="809f7-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="809f7-134">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="809f7-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="809f7-135">响应</span><span class="sxs-lookup"><span data-stu-id="809f7-135">Response</span></span>

<span data-ttu-id="809f7-136">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[mailFolder](../resources/mailfolder.md)资源。</span><span class="sxs-lookup"><span data-stu-id="809f7-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="809f7-137">示例</span><span class="sxs-lookup"><span data-stu-id="809f7-137">Example</span></span>

<span data-ttu-id="809f7-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="809f7-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="809f7-139">请求</span><span class="sxs-lookup"><span data-stu-id="809f7-139">Request</span></span>
<span data-ttu-id="809f7-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="809f7-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="809f7-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="809f7-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="809f7-142">C#</span><span class="sxs-lookup"><span data-stu-id="809f7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="809f7-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="809f7-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="809f7-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="809f7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="809f7-145">Java</span><span class="sxs-lookup"><span data-stu-id="809f7-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="809f7-146">响应</span><span class="sxs-lookup"><span data-stu-id="809f7-146">Response</span></span>

<span data-ttu-id="809f7-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="809f7-147">Here is an example of the response.</span></span>

> <span data-ttu-id="809f7-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="809f7-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="809f7-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="809f7-149">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
