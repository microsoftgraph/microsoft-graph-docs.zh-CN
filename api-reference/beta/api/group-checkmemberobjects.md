---
title: 组： checkMemberObjects
description: 检查指定的组对象的组、目录角色或管理单位列表中的成员身份。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45842a31bb4e7a7b2ec3e5405aa17c4cf6a5a53d
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041804"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="4682a-103">组： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="4682a-103">group: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4682a-104">检查指定组的组列表或管理单元的成员资格。</span><span class="sxs-lookup"><span data-stu-id="4682a-104">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="4682a-105">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="4682a-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4682a-106">权限</span><span class="sxs-lookup"><span data-stu-id="4682a-106">Permissions</span></span>

<span data-ttu-id="4682a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4682a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4682a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4682a-109">Permission type</span></span>                        | <span data-ttu-id="4682a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4682a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4682a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4682a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4682a-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4682a-112">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="4682a-113">并</span><span class="sxs-lookup"><span data-stu-id="4682a-113">And:</span></span><br><ul><li><span data-ttu-id="4682a-114">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="4682a-114">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="4682a-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4682a-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="4682a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4682a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4682a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4682a-117">Not supported.</span></span> |
| <span data-ttu-id="4682a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4682a-118">Application</span></span>                            | <span data-ttu-id="4682a-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4682a-119">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="4682a-120">并</span><span class="sxs-lookup"><span data-stu-id="4682a-120">And:</span></span><br><ul><li><span data-ttu-id="4682a-121">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="4682a-121">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="4682a-122">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4682a-122">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4682a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4682a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="4682a-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="4682a-124">Request headers</span></span>

| <span data-ttu-id="4682a-125">名称</span><span class="sxs-lookup"><span data-stu-id="4682a-125">Name</span></span>          | <span data-ttu-id="4682a-126">说明</span><span class="sxs-lookup"><span data-stu-id="4682a-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4682a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4682a-127">Authorization</span></span> | <span data-ttu-id="4682a-128">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4682a-128">Bearer {token}</span></span> |
| <span data-ttu-id="4682a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4682a-129">Content-Type</span></span>  | <span data-ttu-id="4682a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="4682a-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4682a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="4682a-131">Request body</span></span>

<span data-ttu-id="4682a-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4682a-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4682a-133">参数</span><span class="sxs-lookup"><span data-stu-id="4682a-133">Parameter</span></span>    | <span data-ttu-id="4682a-134">类型</span><span class="sxs-lookup"><span data-stu-id="4682a-134">Type</span></span>        | <span data-ttu-id="4682a-135">说明</span><span class="sxs-lookup"><span data-stu-id="4682a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4682a-136">ids</span><span class="sxs-lookup"><span data-stu-id="4682a-136">ids</span></span>|<span data-ttu-id="4682a-137">String collection</span><span class="sxs-lookup"><span data-stu-id="4682a-137">String collection</span></span>| <span data-ttu-id="4682a-138">包含目录角色的组、目录角色、管理单元或 roleTemplate Id 的对象 Id 的集合，用于检查成员身份。</span><span class="sxs-lookup"><span data-stu-id="4682a-138">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="4682a-139">最高可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="4682a-139">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="4682a-140">响应</span><span class="sxs-lookup"><span data-stu-id="4682a-140">Response</span></span>

<span data-ttu-id="4682a-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="4682a-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4682a-142">示例</span><span class="sxs-lookup"><span data-stu-id="4682a-142">Examples</span></span>

<span data-ttu-id="4682a-143">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4682a-143">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4682a-144">请求</span><span class="sxs-lookup"><span data-stu-id="4682a-144">Request</span></span>

<span data-ttu-id="4682a-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4682a-145">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4682a-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4682a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberObjects
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4682a-147">C#</span><span class="sxs-lookup"><span data-stu-id="4682a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4682a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4682a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4682a-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="4682a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4682a-150">响应</span><span class="sxs-lookup"><span data-stu-id="4682a-150">Response</span></span>

<span data-ttu-id="4682a-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4682a-151">The following is an example of the response.</span></span> 

> <span data-ttu-id="4682a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4682a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
