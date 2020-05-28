---
title: servicePrincipal： getMemberObjects
description: 获取此服务主体所属的组和目录角色列表。  此检查是可传递的。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 76c25cfccb0455db4e6c5837fdb627ac067a3d3c
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383999"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="5beb0-104">servicePrincipal： getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="5beb0-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="5beb0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5beb0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5beb0-106">获取此[servicePrincipal](../resources/serviceprincipal.md)所属的组和目录角色的列表。</span><span class="sxs-lookup"><span data-stu-id="5beb0-106">Get the list of groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="5beb0-107">此检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="5beb0-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5beb0-108">权限</span><span class="sxs-lookup"><span data-stu-id="5beb0-108">Permissions</span></span>
<span data-ttu-id="5beb0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5beb0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5beb0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5beb0-111">Permission type</span></span>      | <span data-ttu-id="5beb0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5beb0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5beb0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5beb0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5beb0-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5beb0-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5beb0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5beb0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5beb0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5beb0-116">Not supported.</span></span>    |
|<span data-ttu-id="5beb0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5beb0-117">Application</span></span> | <span data-ttu-id="5beb0-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5beb0-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5beb0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5beb0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="5beb0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5beb0-120">Request headers</span></span>
| <span data-ttu-id="5beb0-121">名称</span><span class="sxs-lookup"><span data-stu-id="5beb0-121">Name</span></span>       | <span data-ttu-id="5beb0-122">说明</span><span class="sxs-lookup"><span data-stu-id="5beb0-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5beb0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5beb0-123">Authorization</span></span> | <span data-ttu-id="5beb0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5beb0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5beb0-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="5beb0-126">Content-type</span></span> | <span data-ttu-id="5beb0-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5beb0-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5beb0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5beb0-129">Request body</span></span>
<span data-ttu-id="5beb0-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5beb0-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5beb0-131">参数</span><span class="sxs-lookup"><span data-stu-id="5beb0-131">Parameter</span></span>    | <span data-ttu-id="5beb0-132">类型</span><span class="sxs-lookup"><span data-stu-id="5beb0-132">Type</span></span>   |<span data-ttu-id="5beb0-133">Description</span><span class="sxs-lookup"><span data-stu-id="5beb0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5beb0-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="5beb0-134">securityEnabledOnly</span></span>|<span data-ttu-id="5beb0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5beb0-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="5beb0-136">响应</span><span class="sxs-lookup"><span data-stu-id="5beb0-136">Response</span></span>

<span data-ttu-id="5beb0-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="5beb0-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5beb0-138">示例</span><span class="sxs-lookup"><span data-stu-id="5beb0-138">Examples</span></span>
<span data-ttu-id="5beb0-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5beb0-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="5beb0-140">请求</span><span class="sxs-lookup"><span data-stu-id="5beb0-140">Request</span></span>
<span data-ttu-id="5beb0-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5beb0-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5beb0-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5beb0-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="5beb0-143">C#</span><span class="sxs-lookup"><span data-stu-id="5beb0-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5beb0-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5beb0-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5beb0-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5beb0-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5beb0-146">Java</span><span class="sxs-lookup"><span data-stu-id="5beb0-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5beb0-147">响应</span><span class="sxs-lookup"><span data-stu-id="5beb0-147">Response</span></span>
<span data-ttu-id="5beb0-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5beb0-148">Here is an example of the response.</span></span> 
><span data-ttu-id="5beb0-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5beb0-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
