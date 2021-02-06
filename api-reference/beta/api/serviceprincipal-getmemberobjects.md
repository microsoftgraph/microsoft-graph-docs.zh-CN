---
title: 'servicePrincipal: getMemberObjects'
description: 获取此服务主体所属的组和目录角色列表。  此检查是可传递的。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 8ac82717a29aadd8b2623598bd2bc97345ba263a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134433"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="535ed-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="535ed-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="535ed-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="535ed-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="535ed-106">获取此 [servicePrincipal](../resources/serviceprincipal.md)所属的组和目录角色列表。</span><span class="sxs-lookup"><span data-stu-id="535ed-106">Get the list of groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="535ed-107">此检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="535ed-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="535ed-108">权限</span><span class="sxs-lookup"><span data-stu-id="535ed-108">Permissions</span></span>
<span data-ttu-id="535ed-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="535ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535ed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="535ed-111">Permission type</span></span>      | <span data-ttu-id="535ed-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="535ed-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="535ed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="535ed-113">Delegated (work or school account)</span></span> | <span data-ttu-id="535ed-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="535ed-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="535ed-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="535ed-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="535ed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="535ed-116">Not supported.</span></span>    |
|<span data-ttu-id="535ed-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="535ed-117">Application</span></span> | <span data-ttu-id="535ed-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535ed-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="535ed-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="535ed-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="535ed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="535ed-120">Request headers</span></span>
| <span data-ttu-id="535ed-121">名称</span><span class="sxs-lookup"><span data-stu-id="535ed-121">Name</span></span>       | <span data-ttu-id="535ed-122">说明</span><span class="sxs-lookup"><span data-stu-id="535ed-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="535ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="535ed-123">Authorization</span></span> | <span data-ttu-id="535ed-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="535ed-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="535ed-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="535ed-126">Content-type</span></span> | <span data-ttu-id="535ed-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="535ed-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="535ed-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="535ed-129">Request body</span></span>
<span data-ttu-id="535ed-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="535ed-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="535ed-131">参数</span><span class="sxs-lookup"><span data-stu-id="535ed-131">Parameter</span></span>    | <span data-ttu-id="535ed-132">类型</span><span class="sxs-lookup"><span data-stu-id="535ed-132">Type</span></span>   |<span data-ttu-id="535ed-133">说明</span><span class="sxs-lookup"><span data-stu-id="535ed-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="535ed-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="535ed-134">securityEnabledOnly</span></span>|<span data-ttu-id="535ed-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="535ed-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="535ed-136">响应</span><span class="sxs-lookup"><span data-stu-id="535ed-136">Response</span></span>

<span data-ttu-id="535ed-137">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="535ed-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="535ed-138">示例</span><span class="sxs-lookup"><span data-stu-id="535ed-138">Examples</span></span>
<span data-ttu-id="535ed-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="535ed-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="535ed-140">请求</span><span class="sxs-lookup"><span data-stu-id="535ed-140">Request</span></span>
<span data-ttu-id="535ed-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="535ed-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="535ed-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="535ed-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="535ed-143">C#</span><span class="sxs-lookup"><span data-stu-id="535ed-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="535ed-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="535ed-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="535ed-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="535ed-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="535ed-146">Java</span><span class="sxs-lookup"><span data-stu-id="535ed-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="535ed-147">响应</span><span class="sxs-lookup"><span data-stu-id="535ed-147">Response</span></span>
<span data-ttu-id="535ed-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="535ed-148">Here is an example of the response.</span></span> 
><span data-ttu-id="535ed-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="535ed-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



