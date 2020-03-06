---
title: 设备： checkMemberObjects
description: 检查指定的设备对象的组或目录角色列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b432947a9696e4f2ac3c13636356d789594d6d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518145"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="b661b-103">设备： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b661b-103">device: checkMemberObjects</span></span>

<span data-ttu-id="b661b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b661b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b661b-105">检查指定的设备对象的组或目录角色列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="b661b-105">Check for membership in a list of groups or directory roles for the specified device object.</span></span> <span data-ttu-id="b661b-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b661b-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b661b-107">权限</span><span class="sxs-lookup"><span data-stu-id="b661b-107">Permissions</span></span>

<span data-ttu-id="b661b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b661b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b661b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b661b-110">Permission type</span></span>                        | <span data-ttu-id="b661b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b661b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b661b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b661b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b661b-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b661b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b661b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b661b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b661b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b661b-115">Not supported.</span></span> |
| <span data-ttu-id="b661b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b661b-116">Application</span></span>                            | <span data-ttu-id="b661b-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b661b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b661b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b661b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="b661b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b661b-119">Request headers</span></span>

| <span data-ttu-id="b661b-120">名称</span><span class="sxs-lookup"><span data-stu-id="b661b-120">Name</span></span>          | <span data-ttu-id="b661b-121">说明</span><span class="sxs-lookup"><span data-stu-id="b661b-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b661b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b661b-122">Authorization</span></span> | <span data-ttu-id="b661b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b661b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b661b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b661b-125">Content-Type</span></span>  | <span data-ttu-id="b661b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b661b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b661b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b661b-128">Request body</span></span>

<span data-ttu-id="b661b-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b661b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b661b-130">参数</span><span class="sxs-lookup"><span data-stu-id="b661b-130">Parameter</span></span>    | <span data-ttu-id="b661b-131">类型</span><span class="sxs-lookup"><span data-stu-id="b661b-131">Type</span></span>        | <span data-ttu-id="b661b-132">说明</span><span class="sxs-lookup"><span data-stu-id="b661b-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b661b-133">ids</span><span class="sxs-lookup"><span data-stu-id="b661b-133">ids</span></span> | <span data-ttu-id="b661b-134">String collection</span><span class="sxs-lookup"><span data-stu-id="b661b-134">String collection</span></span> | <span data-ttu-id="b661b-135">一个集合，包含要检查其成员身份的目录角色的组、目录角色或 roleTemplate Id 的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="b661b-135">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="b661b-136">最大可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="b661b-136">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="b661b-137">响应</span><span class="sxs-lookup"><span data-stu-id="b661b-137">Response</span></span>

<span data-ttu-id="b661b-138">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="b661b-138">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b661b-139">示例</span><span class="sxs-lookup"><span data-stu-id="b661b-139">Examples</span></span>

<span data-ttu-id="b661b-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b661b-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b661b-141">请求</span><span class="sxs-lookup"><span data-stu-id="b661b-141">Request</span></span>

<span data-ttu-id="b661b-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b661b-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b661b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b661b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "device_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/devices/{id}/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="b661b-144">C#</span><span class="sxs-lookup"><span data-stu-id="b661b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/device-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b661b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b661b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/device-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b661b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b661b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/device-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b661b-147">Java</span><span class="sxs-lookup"><span data-stu-id="b661b-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/device-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b661b-148">响应</span><span class="sxs-lookup"><span data-stu-id="b661b-148">Response</span></span>

<span data-ttu-id="b661b-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b661b-149">The following is an example of the response.</span></span> 

> <span data-ttu-id="b661b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b661b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
