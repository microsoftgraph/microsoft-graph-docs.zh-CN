---
title: 删除所有者
description: 从应用程序删除所有者。
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 034e8299ec1a5a05f1fa307f0196aed2113aebbc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786073"
---
# <a name="remove-owner"></a><span data-ttu-id="85b18-103">删除所有者</span><span class="sxs-lookup"><span data-stu-id="85b18-103">Remove owner</span></span>

<span data-ttu-id="85b18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85b18-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85b18-105">从应用程序中删除 [所有者](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="85b18-105">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85b18-106">权限</span><span class="sxs-lookup"><span data-stu-id="85b18-106">Permissions</span></span>
<span data-ttu-id="85b18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85b18-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="85b18-109">Permission type</span></span>      | <span data-ttu-id="85b18-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85b18-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85b18-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85b18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85b18-112">Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85b18-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="85b18-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85b18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85b18-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="85b18-114">Not supported.</span></span>    |
|<span data-ttu-id="85b18-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="85b18-115">Application</span></span> | <span data-ttu-id="85b18-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="85b18-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85b18-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85b18-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="85b18-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="85b18-118">Request headers</span></span>
| <span data-ttu-id="85b18-119">名称</span><span class="sxs-lookup"><span data-stu-id="85b18-119">Name</span></span> | <span data-ttu-id="85b18-120">说明</span><span class="sxs-lookup"><span data-stu-id="85b18-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="85b18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="85b18-121">Authorization</span></span> | <span data-ttu-id="85b18-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="85b18-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85b18-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="85b18-124">Request body</span></span>
<span data-ttu-id="85b18-125">在请求正文中，提供要分配为所有者的目录对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="85b18-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="85b18-126">响应</span><span class="sxs-lookup"><span data-stu-id="85b18-126">Response</span></span>

<span data-ttu-id="85b18-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="85b18-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="85b18-128">示例</span><span class="sxs-lookup"><span data-stu-id="85b18-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="85b18-129">请求</span><span class="sxs-lookup"><span data-stu-id="85b18-129">Request</span></span>

<span data-ttu-id="85b18-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="85b18-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85b18-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="85b18-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="85b18-132">C#</span><span class="sxs-lookup"><span data-stu-id="85b18-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85b18-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85b18-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85b18-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85b18-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85b18-135">Java</span><span class="sxs-lookup"><span data-stu-id="85b18-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85b18-136">响应</span><span class="sxs-lookup"><span data-stu-id="85b18-136">Response</span></span>

<span data-ttu-id="85b18-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="85b18-137">The following is an example of the response.</span></span>

><span data-ttu-id="85b18-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="85b18-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

