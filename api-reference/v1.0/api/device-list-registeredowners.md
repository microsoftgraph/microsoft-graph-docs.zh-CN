---
title: 列出 registeredOwner
description: 检索身份为已注册设备的所有者的用户列表。
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 198655463c227fa5f0b7b547e59c9f11b08b7571
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434585"
---
# <a name="list-registeredowners"></a><span data-ttu-id="46527-103">列出 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="46527-103">List registeredOwners</span></span>

<span data-ttu-id="46527-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46527-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46527-105">检索身份为已注册设备的所有者的用户列表。</span><span class="sxs-lookup"><span data-stu-id="46527-105">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="46527-106">已注册的所有者是云加入设备或已注册个人设备的用户。</span><span class="sxs-lookup"><span data-stu-id="46527-106">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="46527-107">已注册的所有者是在注册时设置。</span><span class="sxs-lookup"><span data-stu-id="46527-107">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="46527-108">目前，只能有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="46527-108">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="46527-109">权限</span><span class="sxs-lookup"><span data-stu-id="46527-109">Permissions</span></span>
<span data-ttu-id="46527-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46527-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="46527-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="46527-112">Permission type</span></span>      | <span data-ttu-id="46527-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46527-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46527-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46527-114">Delegated (work or school account)</span></span> | <span data-ttu-id="46527-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46527-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46527-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46527-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46527-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="46527-117">Not supported.</span></span>    |
|<span data-ttu-id="46527-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="46527-118">Application</span></span> | <span data-ttu-id="46527-119">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46527-119">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="46527-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46527-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46527-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46527-121">Optional query parameters</span></span>
<span data-ttu-id="46527-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46527-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="46527-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="46527-123">Request headers</span></span>
| <span data-ttu-id="46527-124">名称</span><span class="sxs-lookup"><span data-stu-id="46527-124">Name</span></span>       | <span data-ttu-id="46527-125">类型</span><span class="sxs-lookup"><span data-stu-id="46527-125">Type</span></span> | <span data-ttu-id="46527-126">说明</span><span class="sxs-lookup"><span data-stu-id="46527-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="46527-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="46527-127">Authorization</span></span>  | <span data-ttu-id="46527-128">string</span><span class="sxs-lookup"><span data-stu-id="46527-128">string</span></span>  | <span data-ttu-id="46527-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46527-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46527-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="46527-131">Request body</span></span>
<span data-ttu-id="46527-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46527-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46527-133">响应</span><span class="sxs-lookup"><span data-stu-id="46527-133">Response</span></span>

<span data-ttu-id="46527-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46527-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46527-135">示例</span><span class="sxs-lookup"><span data-stu-id="46527-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46527-136">请求</span><span class="sxs-lookup"><span data-stu-id="46527-136">Request</span></span>
<span data-ttu-id="46527-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46527-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46527-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="46527-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="46527-139">C#</span><span class="sxs-lookup"><span data-stu-id="46527-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46527-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46527-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46527-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46527-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46527-142">Java</span><span class="sxs-lookup"><span data-stu-id="46527-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="46527-143">响应</span><span class="sxs-lookup"><span data-stu-id="46527-143">Response</span></span>
<span data-ttu-id="46527-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46527-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
