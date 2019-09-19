---
title: servicePrincipal： checkMemberObjects
description: 检查指定的服务主体对象的组、目录角色或管理单位列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 512582a8f8413867aeff0ce168c5b5748ed38fc7
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041852"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="57017-103">servicePrincipal： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="57017-103">servicePrincipal: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57017-104">检查指定的服务主体对象的组、目录角色或管理单位列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="57017-104">Check for membership in a list of groups, directory roles, or administrative units for the specified service principle object.</span></span> <span data-ttu-id="57017-105">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="57017-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="57017-106">权限</span><span class="sxs-lookup"><span data-stu-id="57017-106">Permissions</span></span>

<span data-ttu-id="57017-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57017-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57017-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="57017-109">Permission type</span></span>                        | <span data-ttu-id="57017-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57017-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57017-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57017-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="57017-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="57017-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="57017-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57017-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57017-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="57017-114">Not supported.</span></span> |
| <span data-ttu-id="57017-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="57017-115">Application</span></span>                            | <span data-ttu-id="57017-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57017-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57017-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57017-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="57017-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="57017-118">Request headers</span></span>

| <span data-ttu-id="57017-119">名称</span><span class="sxs-lookup"><span data-stu-id="57017-119">Name</span></span>          | <span data-ttu-id="57017-120">说明</span><span class="sxs-lookup"><span data-stu-id="57017-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="57017-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="57017-121">Authorization</span></span> | <span data-ttu-id="57017-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="57017-122">Bearer {token}</span></span> |
| <span data-ttu-id="57017-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57017-123">Content-Type</span></span>  | <span data-ttu-id="57017-124">application/json</span><span class="sxs-lookup"><span data-stu-id="57017-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="57017-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="57017-125">Request body</span></span>

<span data-ttu-id="57017-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="57017-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57017-127">参数</span><span class="sxs-lookup"><span data-stu-id="57017-127">Parameter</span></span>    | <span data-ttu-id="57017-128">类型</span><span class="sxs-lookup"><span data-stu-id="57017-128">Type</span></span>        | <span data-ttu-id="57017-129">说明</span><span class="sxs-lookup"><span data-stu-id="57017-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="57017-130">ids</span><span class="sxs-lookup"><span data-stu-id="57017-130">ids</span></span>|<span data-ttu-id="57017-131">String collection</span><span class="sxs-lookup"><span data-stu-id="57017-131">String collection</span></span>|<span data-ttu-id="57017-132">包含目录角色的组、目录角色、管理单元或 roleTemplate Id 的对象 Id 的集合，用于检查成员身份。</span><span class="sxs-lookup"><span data-stu-id="57017-132">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="57017-133">最高可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="57017-133">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="57017-134">响应</span><span class="sxs-lookup"><span data-stu-id="57017-134">Response</span></span>

<span data-ttu-id="57017-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="57017-135">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57017-136">示例</span><span class="sxs-lookup"><span data-stu-id="57017-136">Examples</span></span>

<span data-ttu-id="57017-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="57017-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="57017-138">请求</span><span class="sxs-lookup"><span data-stu-id="57017-138">Request</span></span>

<span data-ttu-id="57017-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57017-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="57017-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="57017-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="57017-141">C#</span><span class="sxs-lookup"><span data-stu-id="57017-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57017-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57017-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57017-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="57017-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57017-144">响应</span><span class="sxs-lookup"><span data-stu-id="57017-144">Response</span></span>

<span data-ttu-id="57017-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57017-145">The following is an example of the response.</span></span> 

> <span data-ttu-id="57017-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="57017-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
