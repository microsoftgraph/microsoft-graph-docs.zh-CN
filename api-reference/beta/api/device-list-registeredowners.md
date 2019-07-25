---
title: 列出 registeredOwner
description: 检索身份为已注册设备的所有者的用户列表。 已注册的所有者是云加入设备或已注册个人设备的用户。 已注册的所有者是在注册时设置。 目前，只能有一个所有者。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 479901336f2f38b57aff268e90e0fcd3b7a96f5f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862716"
---
# <a name="list-registeredowners"></a><span data-ttu-id="f569c-106">列出 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="f569c-106">List registeredOwners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f569c-107">检索身份为已注册设备的所有者的用户列表。</span><span class="sxs-lookup"><span data-stu-id="f569c-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="f569c-108">已注册的所有者是云加入设备或已注册个人设备的用户。</span><span class="sxs-lookup"><span data-stu-id="f569c-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="f569c-109">已注册的所有者是在注册时设置。</span><span class="sxs-lookup"><span data-stu-id="f569c-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="f569c-110">目前，只能有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="f569c-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="f569c-111">权限</span><span class="sxs-lookup"><span data-stu-id="f569c-111">Permissions</span></span>

<span data-ttu-id="f569c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f569c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f569c-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f569c-114">Permission type</span></span>      | <span data-ttu-id="f569c-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f569c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f569c-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f569c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f569c-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f569c-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f569c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f569c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f569c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f569c-119">Not supported.</span></span>    |
|<span data-ttu-id="f569c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f569c-120">Application</span></span> | <span data-ttu-id="f569c-121">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f569c-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f569c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f569c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="f569c-123">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="f569c-123">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f569c-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f569c-124">Optional query parameters</span></span>
<span data-ttu-id="f569c-125">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f569c-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f569c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="f569c-126">Request headers</span></span>
| <span data-ttu-id="f569c-127">名称</span><span class="sxs-lookup"><span data-stu-id="f569c-127">Name</span></span>       | <span data-ttu-id="f569c-128">类型</span><span class="sxs-lookup"><span data-stu-id="f569c-128">Type</span></span> | <span data-ttu-id="f569c-129">说明</span><span class="sxs-lookup"><span data-stu-id="f569c-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f569c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f569c-130">Authorization</span></span>  | <span data-ttu-id="f569c-131">string</span><span class="sxs-lookup"><span data-stu-id="f569c-131">string</span></span>  | <span data-ttu-id="f569c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f569c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f569c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="f569c-134">Request body</span></span>
<span data-ttu-id="f569c-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f569c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f569c-136">响应</span><span class="sxs-lookup"><span data-stu-id="f569c-136">Response</span></span>

<span data-ttu-id="f569c-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f569c-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f569c-138">示例</span><span class="sxs-lookup"><span data-stu-id="f569c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f569c-139">请求</span><span class="sxs-lookup"><span data-stu-id="f569c-139">Request</span></span>
<span data-ttu-id="f569c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f569c-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f569c-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f569c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f569c-142">C#</span><span class="sxs-lookup"><span data-stu-id="f569c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f569c-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="f569c-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f569c-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="f569c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f569c-145">Java</span><span class="sxs-lookup"><span data-stu-id="f569c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f569c-146">响应</span><span class="sxs-lookup"><span data-stu-id="f569c-146">Response</span></span>
<span data-ttu-id="f569c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f569c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
