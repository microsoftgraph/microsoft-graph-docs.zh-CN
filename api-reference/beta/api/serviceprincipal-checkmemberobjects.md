---
title: servicePrincipal： checkMemberObjects
description: 检查指定的服务主体对象的组、目录角色或管理单位列表中的成员资格。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c70bc51af3a26d00b48ccf97302c9754fff9efd6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334041"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="59edb-103">servicePrincipal： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="59edb-103">servicePrincipal: checkMemberObjects</span></span>

<span data-ttu-id="59edb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59edb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59edb-105">检查指定的[servicePrincipal](../resources/serviceprincipal.md)对象的组、目录角色或管理单位列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="59edb-105">Check for membership in a list of groups, directory roles, or administrative units for the specified [servicePrincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="59edb-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="59edb-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="59edb-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="59edb-107">Permissions</span></span>

<span data-ttu-id="59edb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59edb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59edb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="59edb-110">Permission type</span></span>                        | <span data-ttu-id="59edb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59edb-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="59edb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59edb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="59edb-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="59edb-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="59edb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59edb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59edb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59edb-115">Not supported.</span></span> |
| <span data-ttu-id="59edb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="59edb-116">Application</span></span>                            | <span data-ttu-id="59edb-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59edb-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59edb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59edb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="59edb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59edb-119">Request headers</span></span>

| <span data-ttu-id="59edb-120">名称</span><span class="sxs-lookup"><span data-stu-id="59edb-120">Name</span></span>          | <span data-ttu-id="59edb-121">说明</span><span class="sxs-lookup"><span data-stu-id="59edb-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="59edb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59edb-122">Authorization</span></span> | <span data-ttu-id="59edb-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="59edb-123">Bearer {token}</span></span> |
| <span data-ttu-id="59edb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59edb-124">Content-Type</span></span>  | <span data-ttu-id="59edb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59edb-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="59edb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="59edb-126">Request body</span></span>

<span data-ttu-id="59edb-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="59edb-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59edb-128">参数</span><span class="sxs-lookup"><span data-stu-id="59edb-128">Parameter</span></span>    | <span data-ttu-id="59edb-129">类型</span><span class="sxs-lookup"><span data-stu-id="59edb-129">Type</span></span>        | <span data-ttu-id="59edb-130">Description</span><span class="sxs-lookup"><span data-stu-id="59edb-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59edb-131">ids</span><span class="sxs-lookup"><span data-stu-id="59edb-131">ids</span></span>|<span data-ttu-id="59edb-132">String collection</span><span class="sxs-lookup"><span data-stu-id="59edb-132">String collection</span></span>|<span data-ttu-id="59edb-133">包含目录角色的组、目录角色、管理单元或 roleTemplate Id 的对象 Id 的集合，用于检查成员身份。</span><span class="sxs-lookup"><span data-stu-id="59edb-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="59edb-134">最高可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="59edb-134">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="59edb-135">响应</span><span class="sxs-lookup"><span data-stu-id="59edb-135">Response</span></span>

<span data-ttu-id="59edb-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="59edb-136">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59edb-137">示例</span><span class="sxs-lookup"><span data-stu-id="59edb-137">Examples</span></span>

<span data-ttu-id="59edb-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="59edb-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="59edb-139">请求</span><span class="sxs-lookup"><span data-stu-id="59edb-139">Request</span></span>

<span data-ttu-id="59edb-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="59edb-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="59edb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="59edb-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="59edb-142">C#</span><span class="sxs-lookup"><span data-stu-id="59edb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59edb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59edb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59edb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59edb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59edb-145">响应</span><span class="sxs-lookup"><span data-stu-id="59edb-145">Response</span></span>

<span data-ttu-id="59edb-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="59edb-146">The following is an example of the response.</span></span> 

> <span data-ttu-id="59edb-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="59edb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
