---
title: servicePrincipal：getMemberGroups
description: 获取此服务主体所属的组列表。  检查是可传递的。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 66298b90fb794fc4453de5b983b1213a8486cc23
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134447"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="63750-104">servicePrincipal：getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="63750-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="63750-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63750-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63750-106">获取此[服务主体](../resources/serviceprincipal.md)所属的组列表。</span><span class="sxs-lookup"><span data-stu-id="63750-106">Get the list of groups that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="63750-107">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="63750-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="63750-108">权限</span><span class="sxs-lookup"><span data-stu-id="63750-108">Permissions</span></span>
<span data-ttu-id="63750-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63750-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="63750-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63750-111">Permission type</span></span>      | <span data-ttu-id="63750-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63750-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63750-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63750-113">Delegated (work or school account)</span></span> | <span data-ttu-id="63750-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63750-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63750-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63750-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63750-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63750-116">Not supported.</span></span>    |
|<span data-ttu-id="63750-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="63750-117">Application</span></span> | <span data-ttu-id="63750-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63750-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63750-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63750-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="63750-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="63750-120">Request headers</span></span>
| <span data-ttu-id="63750-121">名称</span><span class="sxs-lookup"><span data-stu-id="63750-121">Name</span></span>       | <span data-ttu-id="63750-122">说明</span><span class="sxs-lookup"><span data-stu-id="63750-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="63750-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63750-123">Authorization</span></span> | <span data-ttu-id="63750-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63750-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="63750-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="63750-126">Content-type</span></span> | <span data-ttu-id="63750-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="63750-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63750-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="63750-129">Request body</span></span>
<span data-ttu-id="63750-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="63750-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63750-131">参数</span><span class="sxs-lookup"><span data-stu-id="63750-131">Parameter</span></span>    | <span data-ttu-id="63750-132">类型</span><span class="sxs-lookup"><span data-stu-id="63750-132">Type</span></span>   |<span data-ttu-id="63750-133">说明</span><span class="sxs-lookup"><span data-stu-id="63750-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63750-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="63750-134">securityEnabledOnly</span></span>|<span data-ttu-id="63750-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="63750-135">Boolean</span></span>|<span data-ttu-id="63750-p106">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="63750-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="63750-138">响应</span><span class="sxs-lookup"><span data-stu-id="63750-138">Response</span></span>

<span data-ttu-id="63750-139">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="63750-139">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63750-140">示例</span><span class="sxs-lookup"><span data-stu-id="63750-140">Examples</span></span>
<span data-ttu-id="63750-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="63750-141">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="63750-142">请求</span><span class="sxs-lookup"><span data-stu-id="63750-142">Request</span></span>
<span data-ttu-id="63750-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63750-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63750-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="63750-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="63750-145">C#</span><span class="sxs-lookup"><span data-stu-id="63750-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63750-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63750-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63750-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63750-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63750-148">Java</span><span class="sxs-lookup"><span data-stu-id="63750-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63750-149">响应</span><span class="sxs-lookup"><span data-stu-id="63750-149">Response</span></span>
<span data-ttu-id="63750-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="63750-150">Here is an example of the response.</span></span> 
><span data-ttu-id="63750-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63750-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



