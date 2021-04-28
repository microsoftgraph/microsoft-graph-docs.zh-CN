---
title: 列出 registeredOwner
description: 检索身份为已注册设备的所有者的用户列表。
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 87c9efd3334703f4f89eca07d13e7ecc2e9b641e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052430"
---
# <a name="list-registeredowners"></a><span data-ttu-id="c158f-103">列出 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="c158f-103">List registeredOwners</span></span>

<span data-ttu-id="c158f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c158f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c158f-105">检索身份为已注册设备的所有者的用户列表。</span><span class="sxs-lookup"><span data-stu-id="c158f-105">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="c158f-106">已注册的所有者是云加入设备或已注册个人设备的用户。</span><span class="sxs-lookup"><span data-stu-id="c158f-106">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="c158f-107">已注册的所有者是在注册时设置。</span><span class="sxs-lookup"><span data-stu-id="c158f-107">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="c158f-108">目前，只能有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="c158f-108">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="c158f-109">权限</span><span class="sxs-lookup"><span data-stu-id="c158f-109">Permissions</span></span>
<span data-ttu-id="c158f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c158f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c158f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c158f-112">Permission type</span></span>      | <span data-ttu-id="c158f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c158f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c158f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c158f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c158f-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c158f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c158f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c158f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c158f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c158f-117">Not supported.</span></span>    |
|<span data-ttu-id="c158f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c158f-118">Application</span></span> | <span data-ttu-id="c158f-119">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c158f-119">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c158f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c158f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c158f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c158f-121">Optional query parameters</span></span>
<span data-ttu-id="c158f-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c158f-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c158f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c158f-123">Request headers</span></span>
| <span data-ttu-id="c158f-124">名称</span><span class="sxs-lookup"><span data-stu-id="c158f-124">Name</span></span>       | <span data-ttu-id="c158f-125">类型</span><span class="sxs-lookup"><span data-stu-id="c158f-125">Type</span></span> | <span data-ttu-id="c158f-126">说明</span><span class="sxs-lookup"><span data-stu-id="c158f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c158f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c158f-127">Authorization</span></span>  | <span data-ttu-id="c158f-128">string</span><span class="sxs-lookup"><span data-stu-id="c158f-128">string</span></span>  | <span data-ttu-id="c158f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c158f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c158f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c158f-131">Request body</span></span>
<span data-ttu-id="c158f-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c158f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c158f-133">响应</span><span class="sxs-lookup"><span data-stu-id="c158f-133">Response</span></span>

<span data-ttu-id="c158f-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c158f-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c158f-135">示例</span><span class="sxs-lookup"><span data-stu-id="c158f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c158f-136">请求</span><span class="sxs-lookup"><span data-stu-id="c158f-136">Request</span></span>
<span data-ttu-id="c158f-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c158f-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c158f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c158f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="c158f-139">C#</span><span class="sxs-lookup"><span data-stu-id="c158f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c158f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c158f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c158f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c158f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c158f-142">Java</span><span class="sxs-lookup"><span data-stu-id="c158f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c158f-143">响应</span><span class="sxs-lookup"><span data-stu-id="c158f-143">Response</span></span>
<span data-ttu-id="c158f-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c158f-144">Here is an example of the response.</span></span> <span data-ttu-id="c158f-145">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c158f-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
