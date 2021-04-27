---
title: orgContact： checkMemberGroups
description: 要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 97e6ce54099301600a0343fe837b947bb0ac18dc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055580"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="ad635-104">orgContact： checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ad635-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="ad635-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad635-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="ad635-106">权限</span><span class="sxs-lookup"><span data-stu-id="ad635-106">Permissions</span></span>
<span data-ttu-id="ad635-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad635-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad635-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad635-109">Permission type</span></span>      | <span data-ttu-id="ad635-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad635-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad635-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad635-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad635-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad635-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad635-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad635-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad635-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad635-114">Not supported.</span></span>    |
|<span data-ttu-id="ad635-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad635-115">Application</span></span> | <span data-ttu-id="ad635-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad635-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad635-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad635-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="ad635-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad635-118">Request headers</span></span>
| <span data-ttu-id="ad635-119">名称</span><span class="sxs-lookup"><span data-stu-id="ad635-119">Name</span></span>       | <span data-ttu-id="ad635-120">类型</span><span class="sxs-lookup"><span data-stu-id="ad635-120">Type</span></span> | <span data-ttu-id="ad635-121">说明</span><span class="sxs-lookup"><span data-stu-id="ad635-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad635-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad635-122">Authorization</span></span>  | <span data-ttu-id="ad635-123">string</span><span class="sxs-lookup"><span data-stu-id="ad635-123">string</span></span>  | <span data-ttu-id="ad635-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad635-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad635-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad635-126">Request body</span></span>
<span data-ttu-id="ad635-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ad635-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ad635-128">参数</span><span class="sxs-lookup"><span data-stu-id="ad635-128">Parameter</span></span>    | <span data-ttu-id="ad635-129">类型</span><span class="sxs-lookup"><span data-stu-id="ad635-129">Type</span></span>   |<span data-ttu-id="ad635-130">说明</span><span class="sxs-lookup"><span data-stu-id="ad635-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad635-131">groupIds</span><span class="sxs-lookup"><span data-stu-id="ad635-131">groupIds</span></span>|<span data-ttu-id="ad635-132">String collection</span><span class="sxs-lookup"><span data-stu-id="ad635-132">String collection</span></span> ||

## <a name="response"></a><span data-ttu-id="ad635-133">响应</span><span class="sxs-lookup"><span data-stu-id="ad635-133">Response</span></span>

<span data-ttu-id="ad635-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="ad635-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad635-135">示例</span><span class="sxs-lookup"><span data-stu-id="ad635-135">Example</span></span>
<span data-ttu-id="ad635-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ad635-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ad635-137">请求</span><span class="sxs-lookup"><span data-stu-id="ad635-137">Request</span></span>
<span data-ttu-id="ad635-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad635-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad635-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad635-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ad635-140">C#</span><span class="sxs-lookup"><span data-stu-id="ad635-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad635-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad635-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad635-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad635-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad635-143">Java</span><span class="sxs-lookup"><span data-stu-id="ad635-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ad635-144">响应</span><span class="sxs-lookup"><span data-stu-id="ad635-144">Response</span></span>
<span data-ttu-id="ad635-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ad635-145">Here is an example of the response.</span></span> <span data-ttu-id="ad635-146">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ad635-146">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


