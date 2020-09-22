---
title: 组： checkMemberObjects
description: 检查指定的组对象的组、目录角色或管理单位列表中的成员身份。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 74fcfe41555ce3b3e8ceb06d02cec11028c655a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990933"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="ff5e3-103">组： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="ff5e3-103">group: checkMemberObjects</span></span>

<span data-ttu-id="ff5e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff5e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff5e3-105">检查指定组的组列表或管理单元的成员资格。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-105">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="ff5e3-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff5e3-107">权限</span><span class="sxs-lookup"><span data-stu-id="ff5e3-107">Permissions</span></span>

<span data-ttu-id="ff5e3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff5e3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff5e3-110">Permission type</span></span>                        | <span data-ttu-id="ff5e3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff5e3-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff5e3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff5e3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff5e3-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5e3-113">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="ff5e3-114">并</span><span class="sxs-lookup"><span data-stu-id="ff5e3-114">And:</span></span><br><ul><li><span data-ttu-id="ff5e3-115">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="ff5e3-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="ff5e3-116">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff5e3-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ff5e3-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff5e3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff5e3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-118">Not supported.</span></span> |
| <span data-ttu-id="ff5e3-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff5e3-119">Application</span></span>                            | <span data-ttu-id="ff5e3-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5e3-120">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="ff5e3-121">并</span><span class="sxs-lookup"><span data-stu-id="ff5e3-121">And:</span></span><br><ul><li><span data-ttu-id="ff5e3-122">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="ff5e3-122">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="ff5e3-123">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5e3-123">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff5e3-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff5e3-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="ff5e3-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff5e3-125">Request headers</span></span>

| <span data-ttu-id="ff5e3-126">名称</span><span class="sxs-lookup"><span data-stu-id="ff5e3-126">Name</span></span>          | <span data-ttu-id="ff5e3-127">说明</span><span class="sxs-lookup"><span data-stu-id="ff5e3-127">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ff5e3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff5e3-128">Authorization</span></span> | <span data-ttu-id="ff5e3-129">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ff5e3-129">Bearer {token}</span></span> |
| <span data-ttu-id="ff5e3-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff5e3-130">Content-Type</span></span>  | <span data-ttu-id="ff5e3-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ff5e3-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff5e3-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff5e3-132">Request body</span></span>

<span data-ttu-id="ff5e3-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ff5e3-134">参数</span><span class="sxs-lookup"><span data-stu-id="ff5e3-134">Parameter</span></span>    | <span data-ttu-id="ff5e3-135">类型</span><span class="sxs-lookup"><span data-stu-id="ff5e3-135">Type</span></span>        | <span data-ttu-id="ff5e3-136">说明</span><span class="sxs-lookup"><span data-stu-id="ff5e3-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff5e3-137">ids</span><span class="sxs-lookup"><span data-stu-id="ff5e3-137">ids</span></span>|<span data-ttu-id="ff5e3-138">String collection</span><span class="sxs-lookup"><span data-stu-id="ff5e3-138">String collection</span></span>| <span data-ttu-id="ff5e3-139">包含目录角色的组、目录角色、管理单元或 roleTemplate Id 的对象 Id 的集合，用于检查成员身份。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-139">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="ff5e3-140">最高可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-140">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="ff5e3-141">响应</span><span class="sxs-lookup"><span data-stu-id="ff5e3-141">Response</span></span>

<span data-ttu-id="ff5e3-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff5e3-143">示例</span><span class="sxs-lookup"><span data-stu-id="ff5e3-143">Examples</span></span>

<span data-ttu-id="ff5e3-144">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-144">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ff5e3-145">请求</span><span class="sxs-lookup"><span data-stu-id="ff5e3-145">Request</span></span>

<span data-ttu-id="ff5e3-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff5e3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff5e3-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ff5e3-148">C#</span><span class="sxs-lookup"><span data-stu-id="ff5e3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff5e3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff5e3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff5e3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff5e3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ff5e3-151">响应</span><span class="sxs-lookup"><span data-stu-id="ff5e3-151">Response</span></span>

<span data-ttu-id="ff5e3-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-152">The following is an example of the response.</span></span> 

> <span data-ttu-id="ff5e3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


