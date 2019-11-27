---
title: 设备： checkMemberObjects
description: 检查指定的设备对象的组或目录角色列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d89ef3e7c78c435f94cceb7b0587c0ff803e28d7
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621577"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="1fa59-103">设备： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="1fa59-103">device: checkMemberObjects</span></span>

<span data-ttu-id="1fa59-104">检查指定的设备对象的组或目录角色列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="1fa59-104">Check for membership in a list of groups or directory roles for the specified device object.</span></span> <span data-ttu-id="1fa59-105">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="1fa59-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fa59-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1fa59-106">Permissions</span></span>

<span data-ttu-id="1fa59-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1fa59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fa59-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fa59-109">Permission type</span></span>                        | <span data-ttu-id="1fa59-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1fa59-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1fa59-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fa59-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fa59-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fa59-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1fa59-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fa59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fa59-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fa59-114">Not supported.</span></span> |
| <span data-ttu-id="1fa59-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fa59-115">Application</span></span>                            | <span data-ttu-id="1fa59-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa59-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fa59-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fa59-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="1fa59-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fa59-118">Request headers</span></span>

| <span data-ttu-id="1fa59-119">名称</span><span class="sxs-lookup"><span data-stu-id="1fa59-119">Name</span></span>          | <span data-ttu-id="1fa59-120">说明</span><span class="sxs-lookup"><span data-stu-id="1fa59-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1fa59-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fa59-121">Authorization</span></span> | <span data-ttu-id="1fa59-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1fa59-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fa59-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fa59-124">Content-Type</span></span>  | <span data-ttu-id="1fa59-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1fa59-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fa59-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fa59-127">Request body</span></span>

<span data-ttu-id="1fa59-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1fa59-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1fa59-129">参数</span><span class="sxs-lookup"><span data-stu-id="1fa59-129">Parameter</span></span>    | <span data-ttu-id="1fa59-130">类型</span><span class="sxs-lookup"><span data-stu-id="1fa59-130">Type</span></span>        | <span data-ttu-id="1fa59-131">说明</span><span class="sxs-lookup"><span data-stu-id="1fa59-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1fa59-132">ids</span><span class="sxs-lookup"><span data-stu-id="1fa59-132">ids</span></span> | <span data-ttu-id="1fa59-133">String collection</span><span class="sxs-lookup"><span data-stu-id="1fa59-133">String collection</span></span> | <span data-ttu-id="1fa59-134">一个集合，包含要检查其成员身份的目录角色的组、目录角色或 roleTemplate Id 的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="1fa59-134">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="1fa59-135">最大可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="1fa59-135">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="1fa59-136">响应</span><span class="sxs-lookup"><span data-stu-id="1fa59-136">Response</span></span>

<span data-ttu-id="1fa59-137">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="1fa59-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fa59-138">示例</span><span class="sxs-lookup"><span data-stu-id="1fa59-138">Examples</span></span>

<span data-ttu-id="1fa59-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1fa59-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1fa59-140">请求</span><span class="sxs-lookup"><span data-stu-id="1fa59-140">Request</span></span>

<span data-ttu-id="1fa59-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1fa59-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1fa59-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fa59-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1fa59-143">C#</span><span class="sxs-lookup"><span data-stu-id="1fa59-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/device-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1fa59-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fa59-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/device-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1fa59-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fa59-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/device-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1fa59-146">Java</span><span class="sxs-lookup"><span data-stu-id="1fa59-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/device-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1fa59-147">响应</span><span class="sxs-lookup"><span data-stu-id="1fa59-147">Response</span></span>

<span data-ttu-id="1fa59-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1fa59-148">The following is an example of the response.</span></span> 

> <span data-ttu-id="1fa59-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1fa59-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
