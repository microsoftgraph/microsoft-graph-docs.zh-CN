---
title: 组： checkMemberObjects
description: 检查指定的组对象的组、目录角色或管理单位列表中的成员身份。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e6d2b4ee6f316d4c11b34940d3bbe9504f2ed67c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954339"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="806ca-103">组： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="806ca-103">group: checkMemberObjects</span></span>

<span data-ttu-id="806ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="806ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="806ca-105">检查指定组的组列表或管理单元的成员资格。</span><span class="sxs-lookup"><span data-stu-id="806ca-105">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="806ca-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="806ca-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="806ca-107">权限</span><span class="sxs-lookup"><span data-stu-id="806ca-107">Permissions</span></span>

<span data-ttu-id="806ca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="806ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="806ca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="806ca-110">Permission type</span></span>                        | <span data-ttu-id="806ca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="806ca-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="806ca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="806ca-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="806ca-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="806ca-113">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="806ca-114">并</span><span class="sxs-lookup"><span data-stu-id="806ca-114">And:</span></span><br><ul><li><span data-ttu-id="806ca-115">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="806ca-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="806ca-116">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="806ca-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="806ca-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="806ca-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="806ca-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="806ca-118">Not supported.</span></span> |
| <span data-ttu-id="806ca-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="806ca-119">Application</span></span>                            | <span data-ttu-id="806ca-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="806ca-120">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="806ca-121">并</span><span class="sxs-lookup"><span data-stu-id="806ca-121">And:</span></span><br><ul><li><span data-ttu-id="806ca-122">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="806ca-122">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="806ca-123">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="806ca-123">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="806ca-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="806ca-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="806ca-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="806ca-125">Request headers</span></span>

| <span data-ttu-id="806ca-126">名称</span><span class="sxs-lookup"><span data-stu-id="806ca-126">Name</span></span>          | <span data-ttu-id="806ca-127">说明</span><span class="sxs-lookup"><span data-stu-id="806ca-127">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="806ca-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="806ca-128">Authorization</span></span> | <span data-ttu-id="806ca-129">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="806ca-129">Bearer {token}</span></span> |
| <span data-ttu-id="806ca-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="806ca-130">Content-Type</span></span>  | <span data-ttu-id="806ca-131">application/json</span><span class="sxs-lookup"><span data-stu-id="806ca-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="806ca-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="806ca-132">Request body</span></span>

<span data-ttu-id="806ca-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="806ca-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="806ca-134">参数</span><span class="sxs-lookup"><span data-stu-id="806ca-134">Parameter</span></span>    | <span data-ttu-id="806ca-135">类型</span><span class="sxs-lookup"><span data-stu-id="806ca-135">Type</span></span>        | <span data-ttu-id="806ca-136">说明</span><span class="sxs-lookup"><span data-stu-id="806ca-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="806ca-137">ids</span><span class="sxs-lookup"><span data-stu-id="806ca-137">ids</span></span>|<span data-ttu-id="806ca-138">String collection</span><span class="sxs-lookup"><span data-stu-id="806ca-138">String collection</span></span>| <span data-ttu-id="806ca-139">包含目录角色的组、目录角色、管理单元或 roleTemplate Id 的对象 Id 的集合，用于检查成员身份。</span><span class="sxs-lookup"><span data-stu-id="806ca-139">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="806ca-140">最高可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="806ca-140">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="806ca-141">响应</span><span class="sxs-lookup"><span data-stu-id="806ca-141">Response</span></span>

<span data-ttu-id="806ca-142">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="806ca-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="806ca-143">示例</span><span class="sxs-lookup"><span data-stu-id="806ca-143">Examples</span></span>

<span data-ttu-id="806ca-144">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="806ca-144">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="806ca-145">请求</span><span class="sxs-lookup"><span data-stu-id="806ca-145">Request</span></span>

<span data-ttu-id="806ca-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="806ca-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="806ca-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="806ca-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="806ca-148">C#</span><span class="sxs-lookup"><span data-stu-id="806ca-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="806ca-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="806ca-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="806ca-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="806ca-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="806ca-151">Java</span><span class="sxs-lookup"><span data-stu-id="806ca-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="806ca-152">响应</span><span class="sxs-lookup"><span data-stu-id="806ca-152">Response</span></span>

<span data-ttu-id="806ca-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="806ca-153">The following is an example of the response.</span></span> 

> <span data-ttu-id="806ca-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="806ca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


