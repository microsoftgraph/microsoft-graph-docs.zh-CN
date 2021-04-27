---
title: device： checkMemberObjects
description: 检查指定设备对象的组、目录角色或管理单元列表中的成员身份。
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 071ce116c26cea3fba8672c62d78fa054946295a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046984"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="57222-103">device： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="57222-103">device: checkMemberObjects</span></span>

<span data-ttu-id="57222-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57222-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57222-105">检查指定设备对象的组或管理单元列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="57222-105">Check for membership in a list of groups or administrative units for the specified device object.</span></span> <span data-ttu-id="57222-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="57222-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="57222-107">权限</span><span class="sxs-lookup"><span data-stu-id="57222-107">Permissions</span></span>

<span data-ttu-id="57222-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57222-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57222-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="57222-110">Permission type</span></span>                        | <span data-ttu-id="57222-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57222-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57222-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57222-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="57222-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="57222-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="57222-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57222-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57222-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57222-115">Not supported.</span></span> |
| <span data-ttu-id="57222-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="57222-116">Application</span></span>                            | <span data-ttu-id="57222-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57222-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57222-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57222-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="57222-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="57222-119">Request headers</span></span>

| <span data-ttu-id="57222-120">名称</span><span class="sxs-lookup"><span data-stu-id="57222-120">Name</span></span>          | <span data-ttu-id="57222-121">说明</span><span class="sxs-lookup"><span data-stu-id="57222-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="57222-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57222-122">Authorization</span></span> | <span data-ttu-id="57222-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="57222-123">Bearer {token}</span></span> |
| <span data-ttu-id="57222-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57222-124">Content-Type</span></span>  | <span data-ttu-id="57222-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57222-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="57222-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="57222-126">Request body</span></span>

<span data-ttu-id="57222-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="57222-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57222-128">参数</span><span class="sxs-lookup"><span data-stu-id="57222-128">Parameter</span></span>    | <span data-ttu-id="57222-129">类型</span><span class="sxs-lookup"><span data-stu-id="57222-129">Type</span></span>        | <span data-ttu-id="57222-130">说明</span><span class="sxs-lookup"><span data-stu-id="57222-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="57222-131">ids</span><span class="sxs-lookup"><span data-stu-id="57222-131">ids</span></span> | <span data-ttu-id="57222-132">String collection</span><span class="sxs-lookup"><span data-stu-id="57222-132">String collection</span></span> | <span data-ttu-id="57222-133">包含要检查成员身份的目录角色的组、目录角色、管理单元或 roleTemplate ID 的对象 ID 的集合。</span><span class="sxs-lookup"><span data-stu-id="57222-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="57222-134">最多可指定 20 个对象。</span><span class="sxs-lookup"><span data-stu-id="57222-134">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="57222-135">响应</span><span class="sxs-lookup"><span data-stu-id="57222-135">Response</span></span>

<span data-ttu-id="57222-136">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="57222-136">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57222-137">示例</span><span class="sxs-lookup"><span data-stu-id="57222-137">Examples</span></span>

<span data-ttu-id="57222-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="57222-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="57222-139">请求</span><span class="sxs-lookup"><span data-stu-id="57222-139">Request</span></span>

<span data-ttu-id="57222-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57222-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57222-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="57222-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "device_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/devices/{id}/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="57222-142">C#</span><span class="sxs-lookup"><span data-stu-id="57222-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/device-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57222-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57222-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/device-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57222-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57222-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/device-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57222-145">Java</span><span class="sxs-lookup"><span data-stu-id="57222-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/device-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57222-146">响应</span><span class="sxs-lookup"><span data-stu-id="57222-146">Response</span></span>

<span data-ttu-id="57222-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57222-147">The following is an example of the response.</span></span> 

> <span data-ttu-id="57222-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="57222-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "device: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


