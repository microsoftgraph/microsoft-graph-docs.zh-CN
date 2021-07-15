---
title: 从 incompatibleAccessPackages 中删除 accessPackage
description: 删除指示访问包与指定访问包不兼容的链接。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c228402a433c3d9920481030ead07e79333459bc
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439356"
---
# <a name="remove-accesspackage-from-incompatibleaccesspackages"></a><span data-ttu-id="66856-103">从 incompatibleAccessPackages 中删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="66856-103">Remove accessPackage from incompatibleAccessPackages</span></span>

<span data-ttu-id="66856-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66856-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66856-105">从 [accessPackage](../resources/accesspackage.md) 上标记为不兼容的访问包列表中删除 [访问包](../resources/accesspackage.md)。</span><span class="sxs-lookup"><span data-stu-id="66856-105">Remove an [access package](../resources/accesspackage.md) from the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="66856-106">权限</span><span class="sxs-lookup"><span data-stu-id="66856-106">Permissions</span></span>

<span data-ttu-id="66856-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66856-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="66856-109">Permission type</span></span>                        | <span data-ttu-id="66856-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66856-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66856-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66856-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="66856-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66856-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="66856-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66856-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66856-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="66856-114">Not supported.</span></span> |
| <span data-ttu-id="66856-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="66856-115">Application</span></span>                            | <span data-ttu-id="66856-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66856-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66856-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66856-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="66856-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="66856-118">Request headers</span></span>

| <span data-ttu-id="66856-119">名称</span><span class="sxs-lookup"><span data-stu-id="66856-119">Name</span></span>          | <span data-ttu-id="66856-120">说明</span><span class="sxs-lookup"><span data-stu-id="66856-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="66856-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66856-121">Authorization</span></span> | <span data-ttu-id="66856-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66856-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66856-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66856-124">Content-Type</span></span>  | <span data-ttu-id="66856-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="66856-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="66856-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="66856-127">Request body</span></span>

<span data-ttu-id="66856-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66856-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66856-129">响应</span><span class="sxs-lookup"><span data-stu-id="66856-129">Response</span></span>

<span data-ttu-id="66856-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="66856-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66856-132">示例</span><span class="sxs-lookup"><span data-stu-id="66856-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66856-133">请求</span><span class="sxs-lookup"><span data-stu-id="66856-133">Request</span></span>

<span data-ttu-id="66856-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66856-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="66856-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="66856-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_incompatibleaccesspackage_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="66856-136">C#</span><span class="sxs-lookup"><span data-stu-id="66856-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-incompatibleaccesspackage-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66856-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66856-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-incompatibleaccesspackage-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66856-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66856-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-incompatibleaccesspackage-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66856-139">Java</span><span class="sxs-lookup"><span data-stu-id="66856-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-incompatibleaccesspackage-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="66856-140">响应</span><span class="sxs-lookup"><span data-stu-id="66856-140">Response</span></span>

<span data-ttu-id="66856-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="66856-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

