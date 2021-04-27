---
title: orgContact： getMemberGroups
description: 要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f9aea52388a64355989ff78c222b00ff893e3473
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055552"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="e6396-104">orgContact： getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e6396-104">orgContact: getMemberGroups</span></span>

<span data-ttu-id="e6396-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6396-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="e6396-106">权限</span><span class="sxs-lookup"><span data-stu-id="e6396-106">Permissions</span></span>
<span data-ttu-id="e6396-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6396-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6396-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6396-109">Permission type</span></span>      | <span data-ttu-id="e6396-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6396-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6396-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6396-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e6396-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6396-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6396-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6396-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6396-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6396-114">Not supported.</span></span>    |
|<span data-ttu-id="e6396-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6396-115">Application</span></span> | <span data-ttu-id="e6396-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6396-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6396-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6396-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="e6396-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6396-118">Request headers</span></span>
| <span data-ttu-id="e6396-119">名称</span><span class="sxs-lookup"><span data-stu-id="e6396-119">Name</span></span>       | <span data-ttu-id="e6396-120">类型</span><span class="sxs-lookup"><span data-stu-id="e6396-120">Type</span></span> | <span data-ttu-id="e6396-121">说明</span><span class="sxs-lookup"><span data-stu-id="e6396-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6396-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6396-122">Authorization</span></span>  | <span data-ttu-id="e6396-123">string</span><span class="sxs-lookup"><span data-stu-id="e6396-123">string</span></span>  | <span data-ttu-id="e6396-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6396-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6396-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6396-126">Request body</span></span>
<span data-ttu-id="e6396-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e6396-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6396-128">参数</span><span class="sxs-lookup"><span data-stu-id="e6396-128">Parameter</span></span>    | <span data-ttu-id="e6396-129">类型</span><span class="sxs-lookup"><span data-stu-id="e6396-129">Type</span></span>   |<span data-ttu-id="e6396-130">说明</span><span class="sxs-lookup"><span data-stu-id="e6396-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6396-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e6396-131">securityEnabledOnly</span></span>|<span data-ttu-id="e6396-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6396-132">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="e6396-133">响应</span><span class="sxs-lookup"><span data-stu-id="e6396-133">Response</span></span>

<span data-ttu-id="e6396-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="e6396-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6396-135">示例</span><span class="sxs-lookup"><span data-stu-id="e6396-135">Example</span></span>
<span data-ttu-id="e6396-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e6396-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6396-137">请求</span><span class="sxs-lookup"><span data-stu-id="e6396-137">Request</span></span>
<span data-ttu-id="e6396-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6396-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6396-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6396-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="e6396-140">C#</span><span class="sxs-lookup"><span data-stu-id="e6396-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6396-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6396-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6396-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6396-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6396-143">Java</span><span class="sxs-lookup"><span data-stu-id="e6396-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e6396-144">响应</span><span class="sxs-lookup"><span data-stu-id="e6396-144">Response</span></span>
<span data-ttu-id="e6396-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e6396-145">Here is an example of the response.</span></span> <span data-ttu-id="e6396-146">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e6396-146">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


