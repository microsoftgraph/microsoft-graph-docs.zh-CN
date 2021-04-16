---
title: servicePrincipal：checkMemberGroups
description: 检查指定组列表中的成员身份。 将列表中具有直接或可传递成员身份的服务主体组返回。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: eef89eadb22b99d2c094f2dabf483edad014e5d2
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870000"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="48121-104">servicePrincipal：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="48121-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="48121-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48121-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48121-106">检查指定组列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="48121-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="48121-107">将列表中具有直接或可传递成员身份的 [servicePrincipal](../resources/serviceprincipal.md) 组返回。</span><span class="sxs-lookup"><span data-stu-id="48121-107">Returns from the list those groups of which the [servicePrincipal](../resources/serviceprincipal.md) has a direct or transitive membership.</span></span>

## <a name="permissions"></a><span data-ttu-id="48121-108">权限</span><span class="sxs-lookup"><span data-stu-id="48121-108">Permissions</span></span>
<span data-ttu-id="48121-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48121-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48121-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="48121-111">Permission type</span></span>      | <span data-ttu-id="48121-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48121-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48121-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48121-113">Delegated (work or school account)</span></span> | <span data-ttu-id="48121-114">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48121-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48121-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48121-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48121-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="48121-116">Not supported.</span></span>    |
|<span data-ttu-id="48121-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="48121-117">Application</span></span> | <span data-ttu-id="48121-118">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48121-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48121-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48121-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="48121-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="48121-120">Request headers</span></span>
| <span data-ttu-id="48121-121">名称</span><span class="sxs-lookup"><span data-stu-id="48121-121">Name</span></span>       | <span data-ttu-id="48121-122">说明</span><span class="sxs-lookup"><span data-stu-id="48121-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="48121-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48121-123">Authorization</span></span> | <span data-ttu-id="48121-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48121-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48121-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48121-126">Content-Type</span></span> | <span data-ttu-id="48121-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="48121-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48121-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="48121-129">Request body</span></span>
<span data-ttu-id="48121-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="48121-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48121-131">参数</span><span class="sxs-lookup"><span data-stu-id="48121-131">Parameter</span></span>    | <span data-ttu-id="48121-132">类型</span><span class="sxs-lookup"><span data-stu-id="48121-132">Type</span></span>   |<span data-ttu-id="48121-133">说明</span><span class="sxs-lookup"><span data-stu-id="48121-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48121-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="48121-134">groupIds</span></span>|<span data-ttu-id="48121-135">String collection</span><span class="sxs-lookup"><span data-stu-id="48121-135">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="48121-136">响应</span><span class="sxs-lookup"><span data-stu-id="48121-136">Response</span></span>

<span data-ttu-id="48121-137">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="48121-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48121-138">示例</span><span class="sxs-lookup"><span data-stu-id="48121-138">Examples</span></span>
<span data-ttu-id="48121-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="48121-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="48121-140">请求</span><span class="sxs-lookup"><span data-stu-id="48121-140">Request</span></span>
<span data-ttu-id="48121-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48121-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="48121-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="48121-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="48121-143">C#</span><span class="sxs-lookup"><span data-stu-id="48121-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48121-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48121-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48121-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48121-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48121-146">Java</span><span class="sxs-lookup"><span data-stu-id="48121-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="48121-147">响应</span><span class="sxs-lookup"><span data-stu-id="48121-147">Response</span></span>
<span data-ttu-id="48121-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="48121-148">Here is an example of the response.</span></span> 
><span data-ttu-id="48121-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48121-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

