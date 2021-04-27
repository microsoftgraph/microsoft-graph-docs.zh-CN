---
title: 创建 Outlook 类别
description: 在用户主类别列表中创建 outlookCategory 对象。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9a0b13fdac001a168d2d43ea6e70e2c3651c0c47
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038017"
---
# <a name="create-outlook-category"></a><span data-ttu-id="3ec4d-103">创建 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="3ec4d-103">Create Outlook category</span></span>

<span data-ttu-id="3ec4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec4d-105">在用户主类别列表中创建 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-105">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ec4d-106">权限</span><span class="sxs-lookup"><span data-stu-id="3ec4d-106">Permissions</span></span>
<span data-ttu-id="3ec4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec4d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ec4d-109">Permission type</span></span>      | <span data-ttu-id="3ec4d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ec4d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ec4d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec4d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ec4d-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec4d-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3ec4d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec4d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec4d-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec4d-114">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="3ec4d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ec4d-115">Application</span></span> | <span data-ttu-id="3ec4d-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec4d-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ec4d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ec4d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="3ec4d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ec4d-118">Request headers</span></span>
| <span data-ttu-id="3ec4d-119">名称</span><span class="sxs-lookup"><span data-stu-id="3ec4d-119">Name</span></span>       | <span data-ttu-id="3ec4d-120">说明</span><span class="sxs-lookup"><span data-stu-id="3ec4d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ec4d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec4d-121">Authorization</span></span>  | <span data-ttu-id="3ec4d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3ec4d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ec4d-124">Request body</span></span>
<span data-ttu-id="3ec4d-125">在请求正文中，提供 [outlookCategory](../resources/outlookcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-125">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ec4d-126">响应</span><span class="sxs-lookup"><span data-stu-id="3ec4d-126">Response</span></span>

<span data-ttu-id="3ec4d-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-127">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ec4d-128">示例</span><span class="sxs-lookup"><span data-stu-id="3ec4d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ec4d-129">请求</span><span class="sxs-lookup"><span data-stu-id="3ec4d-129">Request</span></span>
<span data-ttu-id="3ec4d-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ec4d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec4d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
# <a name="c"></a>[<span data-ttu-id="3ec4d-132">C#</span><span class="sxs-lookup"><span data-stu-id="3ec4d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlookcategory-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ec4d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec4d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlookcategory-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec4d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec4d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlookcategory-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec4d-135">Java</span><span class="sxs-lookup"><span data-stu-id="3ec4d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlookcategory-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3ec4d-136">在请求正文中，提供 [outlookCategory](../resources/outlookcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-136">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3ec4d-137">响应</span><span class="sxs-lookup"><span data-stu-id="3ec4d-137">Response</span></span>
<span data-ttu-id="3ec4d-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-138">Here is an example of the response.</span></span> <span data-ttu-id="3ec4d-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3ec4d-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


