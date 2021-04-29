---
title: 'servicePrincipal: getMemberObjects'
description: 获取此服务主体所属的组和目录角色列表。  此检查是可传递的。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: e379af3615f8cc178a7bef8571e4582dbf4ca0da
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051919"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="d06e6-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="d06e6-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="d06e6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d06e6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d06e6-106">获取此 [servicePrincipal](../resources/serviceprincipal.md)所属的组和目录角色列表。</span><span class="sxs-lookup"><span data-stu-id="d06e6-106">Get the list of groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="d06e6-107">此检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="d06e6-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d06e6-108">权限</span><span class="sxs-lookup"><span data-stu-id="d06e6-108">Permissions</span></span>
<span data-ttu-id="d06e6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d06e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d06e6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d06e6-111">Permission type</span></span>      | <span data-ttu-id="d06e6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d06e6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d06e6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d06e6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d06e6-114">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d06e6-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d06e6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d06e6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d06e6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d06e6-116">Not supported.</span></span>    |
|<span data-ttu-id="d06e6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d06e6-117">Application</span></span> | <span data-ttu-id="d06e6-118">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d06e6-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d06e6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d06e6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="d06e6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d06e6-120">Request headers</span></span>
| <span data-ttu-id="d06e6-121">名称</span><span class="sxs-lookup"><span data-stu-id="d06e6-121">Name</span></span>       | <span data-ttu-id="d06e6-122">说明</span><span class="sxs-lookup"><span data-stu-id="d06e6-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="d06e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d06e6-123">Authorization</span></span> | <span data-ttu-id="d06e6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d06e6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d06e6-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="d06e6-126">Content-type</span></span> | <span data-ttu-id="d06e6-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d06e6-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d06e6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d06e6-129">Request body</span></span>
<span data-ttu-id="d06e6-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d06e6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d06e6-131">参数</span><span class="sxs-lookup"><span data-stu-id="d06e6-131">Parameter</span></span>    | <span data-ttu-id="d06e6-132">类型</span><span class="sxs-lookup"><span data-stu-id="d06e6-132">Type</span></span>   |<span data-ttu-id="d06e6-133">说明</span><span class="sxs-lookup"><span data-stu-id="d06e6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d06e6-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d06e6-134">securityEnabledOnly</span></span>|<span data-ttu-id="d06e6-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d06e6-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="d06e6-136">响应</span><span class="sxs-lookup"><span data-stu-id="d06e6-136">Response</span></span>

<span data-ttu-id="d06e6-137">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="d06e6-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d06e6-138">示例</span><span class="sxs-lookup"><span data-stu-id="d06e6-138">Examples</span></span>
<span data-ttu-id="d06e6-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d06e6-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="d06e6-140">请求</span><span class="sxs-lookup"><span data-stu-id="d06e6-140">Request</span></span>
<span data-ttu-id="d06e6-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d06e6-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d06e6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d06e6-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="d06e6-143">C#</span><span class="sxs-lookup"><span data-stu-id="d06e6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d06e6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d06e6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d06e6-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d06e6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d06e6-146">Java</span><span class="sxs-lookup"><span data-stu-id="d06e6-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d06e6-147">响应</span><span class="sxs-lookup"><span data-stu-id="d06e6-147">Response</span></span>
<span data-ttu-id="d06e6-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d06e6-148">Here is an example of the response.</span></span> 
><span data-ttu-id="d06e6-149">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d06e6-149">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



