---
title: 列出 registeredOwner
description: 检索身份为已注册设备的所有者的用户列表。 已注册的所有者是云加入设备或已注册个人设备的用户。 已注册的所有者是在注册时设置。 目前，只能有一个所有者。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bf56b72389ae3ffebde2dbf27af70f216107e10a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518117"
---
# <a name="list-registeredowners"></a><span data-ttu-id="1d00a-106">列出 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="1d00a-106">List registeredOwners</span></span>

<span data-ttu-id="1d00a-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d00a-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d00a-108">检索身份为已注册设备的所有者的用户列表。</span><span class="sxs-lookup"><span data-stu-id="1d00a-108">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="1d00a-109">已注册的所有者是云加入设备或已注册个人设备的用户。</span><span class="sxs-lookup"><span data-stu-id="1d00a-109">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="1d00a-110">已注册的所有者是在注册时设置。</span><span class="sxs-lookup"><span data-stu-id="1d00a-110">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="1d00a-111">目前，只能有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="1d00a-111">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d00a-112">权限</span><span class="sxs-lookup"><span data-stu-id="1d00a-112">Permissions</span></span>
<span data-ttu-id="1d00a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d00a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d00a-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d00a-115">Permission type</span></span>      | <span data-ttu-id="1d00a-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d00a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d00a-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d00a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1d00a-118">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d00a-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d00a-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d00a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d00a-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d00a-120">Not supported.</span></span>    |
|<span data-ttu-id="1d00a-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d00a-121">Application</span></span> | <span data-ttu-id="1d00a-122">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d00a-122">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1d00a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d00a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d00a-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1d00a-124">Optional query parameters</span></span>
<span data-ttu-id="1d00a-125">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1d00a-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1d00a-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d00a-126">Request headers</span></span>
| <span data-ttu-id="1d00a-127">名称</span><span class="sxs-lookup"><span data-stu-id="1d00a-127">Name</span></span>       | <span data-ttu-id="1d00a-128">类型</span><span class="sxs-lookup"><span data-stu-id="1d00a-128">Type</span></span> | <span data-ttu-id="1d00a-129">说明</span><span class="sxs-lookup"><span data-stu-id="1d00a-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1d00a-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d00a-130">Authorization</span></span>  | <span data-ttu-id="1d00a-131">string</span><span class="sxs-lookup"><span data-stu-id="1d00a-131">string</span></span>  | <span data-ttu-id="1d00a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d00a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d00a-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d00a-134">Request body</span></span>
<span data-ttu-id="1d00a-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1d00a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d00a-136">响应</span><span class="sxs-lookup"><span data-stu-id="1d00a-136">Response</span></span>

<span data-ttu-id="1d00a-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1d00a-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d00a-138">示例</span><span class="sxs-lookup"><span data-stu-id="1d00a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d00a-139">请求</span><span class="sxs-lookup"><span data-stu-id="1d00a-139">Request</span></span>
<span data-ttu-id="1d00a-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d00a-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d00a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d00a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="1d00a-142">C#</span><span class="sxs-lookup"><span data-stu-id="1d00a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d00a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d00a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d00a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d00a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d00a-145">Java</span><span class="sxs-lookup"><span data-stu-id="1d00a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1d00a-146">响应</span><span class="sxs-lookup"><span data-stu-id="1d00a-146">Response</span></span>
<span data-ttu-id="1d00a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d00a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
