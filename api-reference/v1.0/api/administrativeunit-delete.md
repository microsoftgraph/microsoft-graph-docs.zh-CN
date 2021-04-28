---
title: 删除 administrativeUnit
description: 删除 administrativeUnit。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 79739889099924555d5282689ea0baa310bc2844
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054222"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="b9e82-103">删除 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b9e82-103">Delete administrativeUnit</span></span>

<span data-ttu-id="b9e82-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9e82-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9e82-105">删除 [administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="b9e82-105">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e82-106">权限</span><span class="sxs-lookup"><span data-stu-id="b9e82-106">Permissions</span></span>
<span data-ttu-id="b9e82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9e82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b9e82-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e82-109">Permission type</span></span>      | <span data-ttu-id="b9e82-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e82-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9e82-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e82-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9e82-112">AdministrativeUnit.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9e82-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9e82-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e82-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e82-114">Not supported.</span></span>    |
|<span data-ttu-id="b9e82-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e82-115">Application</span></span> | <span data-ttu-id="b9e82-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e82-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9e82-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e82-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b9e82-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e82-118">Request headers</span></span>
| <span data-ttu-id="b9e82-119">名称</span><span class="sxs-lookup"><span data-stu-id="b9e82-119">Name</span></span>       | <span data-ttu-id="b9e82-120">说明</span><span class="sxs-lookup"><span data-stu-id="b9e82-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9e82-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e82-121">Authorization</span></span>  | <span data-ttu-id="b9e82-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e82-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9e82-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e82-124">Request body</span></span>
<span data-ttu-id="b9e82-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9e82-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e82-126">响应</span><span class="sxs-lookup"><span data-stu-id="b9e82-126">Response</span></span>

<span data-ttu-id="b9e82-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b9e82-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e82-129">示例</span><span class="sxs-lookup"><span data-stu-id="b9e82-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9e82-130">请求</span><span class="sxs-lookup"><span data-stu-id="b9e82-130">Request</span></span>
<span data-ttu-id="b9e82-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9e82-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b9e82-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9e82-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="b9e82-133">C#</span><span class="sxs-lookup"><span data-stu-id="b9e82-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9e82-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9e82-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9e82-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9e82-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9e82-136">Java</span><span class="sxs-lookup"><span data-stu-id="b9e82-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="b9e82-137">响应</span><span class="sxs-lookup"><span data-stu-id="b9e82-137">Response</span></span>
<span data-ttu-id="b9e82-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b9e82-138">Here is an example of the response.</span></span> <span data-ttu-id="b9e82-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9e82-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
