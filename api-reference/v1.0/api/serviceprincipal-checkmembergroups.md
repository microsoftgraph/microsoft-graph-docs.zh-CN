---
title: servicePrincipal： checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表中返回，这些组的服务主体具有直接或可传递的成员身份。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bf838a9e13e610ea25d084cbee59c7ad59125ced
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334370"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="20912-104">servicePrincipal： checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="20912-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="20912-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20912-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20912-106">检查指定组列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="20912-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="20912-107">从列表中返回，这些组的[servicePrincipal](../resources/serviceprincipal.md)具有直接或可传递的成员资格。</span><span class="sxs-lookup"><span data-stu-id="20912-107">Returns from the list those groups of which the [servicePrincipal](../resources/serviceprincipal.md) has a direct or transitive membership.</span></span>

## <a name="permissions"></a><span data-ttu-id="20912-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="20912-108">Permissions</span></span>
<span data-ttu-id="20912-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20912-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20912-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="20912-111">Permission type</span></span>      | <span data-ttu-id="20912-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20912-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20912-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20912-113">Delegated (work or school account)</span></span> | <span data-ttu-id="20912-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20912-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20912-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20912-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20912-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20912-116">Not supported.</span></span>    |
|<span data-ttu-id="20912-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="20912-117">Application</span></span> | <span data-ttu-id="20912-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="20912-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20912-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20912-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="20912-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="20912-120">Request headers</span></span>
| <span data-ttu-id="20912-121">名称</span><span class="sxs-lookup"><span data-stu-id="20912-121">Name</span></span>       | <span data-ttu-id="20912-122">说明</span><span class="sxs-lookup"><span data-stu-id="20912-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="20912-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20912-123">Authorization</span></span> | <span data-ttu-id="20912-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20912-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="20912-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20912-126">Content-Type</span></span> | <span data-ttu-id="20912-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="20912-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20912-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="20912-129">Request body</span></span>
<span data-ttu-id="20912-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="20912-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20912-131">参数</span><span class="sxs-lookup"><span data-stu-id="20912-131">Parameter</span></span>    | <span data-ttu-id="20912-132">类型</span><span class="sxs-lookup"><span data-stu-id="20912-132">Type</span></span>   |<span data-ttu-id="20912-133">Description</span><span class="sxs-lookup"><span data-stu-id="20912-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20912-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="20912-134">groupIds</span></span>|<span data-ttu-id="20912-135">String collection</span><span class="sxs-lookup"><span data-stu-id="20912-135">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="20912-136">响应</span><span class="sxs-lookup"><span data-stu-id="20912-136">Response</span></span>

<span data-ttu-id="20912-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="20912-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20912-138">示例</span><span class="sxs-lookup"><span data-stu-id="20912-138">Examples</span></span>
<span data-ttu-id="20912-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="20912-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="20912-140">请求</span><span class="sxs-lookup"><span data-stu-id="20912-140">Request</span></span>
<span data-ttu-id="20912-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20912-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="20912-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="20912-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="20912-143">C#</span><span class="sxs-lookup"><span data-stu-id="20912-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20912-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20912-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20912-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20912-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20912-146">Java</span><span class="sxs-lookup"><span data-stu-id="20912-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="20912-147">响应</span><span class="sxs-lookup"><span data-stu-id="20912-147">Response</span></span>
<span data-ttu-id="20912-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="20912-148">Here is an example of the response.</span></span> 
><span data-ttu-id="20912-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20912-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
