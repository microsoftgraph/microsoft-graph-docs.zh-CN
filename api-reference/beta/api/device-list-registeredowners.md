---
title: 列出 registeredOwner
description: 检索身份为已注册设备的所有者的用户列表。
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c0fb6bd5adcbc6b54ca1d23fb58b51c761d430d
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48371527"
---
# <a name="list-registeredowners"></a><span data-ttu-id="82151-103">列出 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="82151-103">List registeredOwners</span></span>

<span data-ttu-id="82151-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82151-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82151-105">检索身份为已注册设备的所有者的用户列表。</span><span class="sxs-lookup"><span data-stu-id="82151-105">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="82151-106">已注册的所有者是云加入设备或已注册个人设备的用户。</span><span class="sxs-lookup"><span data-stu-id="82151-106">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="82151-107">已注册的所有者是在注册时设置。</span><span class="sxs-lookup"><span data-stu-id="82151-107">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="82151-108">目前，只能有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="82151-108">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="82151-109">权限</span><span class="sxs-lookup"><span data-stu-id="82151-109">Permissions</span></span>

<span data-ttu-id="82151-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82151-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82151-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="82151-112">Permission type</span></span>      | <span data-ttu-id="82151-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82151-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82151-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82151-114">Delegated (work or school account)</span></span> | <span data-ttu-id="82151-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82151-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82151-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82151-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82151-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="82151-117">Not supported.</span></span>    |
|<span data-ttu-id="82151-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="82151-118">Application</span></span> | <span data-ttu-id="82151-119">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82151-119">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="82151-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82151-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="82151-121">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="82151-121">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="82151-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="82151-122">Optional query parameters</span></span>
<span data-ttu-id="82151-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="82151-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="82151-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="82151-124">Request headers</span></span>
| <span data-ttu-id="82151-125">名称</span><span class="sxs-lookup"><span data-stu-id="82151-125">Name</span></span>       | <span data-ttu-id="82151-126">类型</span><span class="sxs-lookup"><span data-stu-id="82151-126">Type</span></span> | <span data-ttu-id="82151-127">说明</span><span class="sxs-lookup"><span data-stu-id="82151-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82151-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="82151-128">Authorization</span></span>  | <span data-ttu-id="82151-129">string</span><span class="sxs-lookup"><span data-stu-id="82151-129">string</span></span>  | <span data-ttu-id="82151-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82151-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82151-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="82151-132">Request body</span></span>
<span data-ttu-id="82151-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82151-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82151-134">响应</span><span class="sxs-lookup"><span data-stu-id="82151-134">Response</span></span>

<span data-ttu-id="82151-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82151-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82151-136">示例</span><span class="sxs-lookup"><span data-stu-id="82151-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82151-137">请求</span><span class="sxs-lookup"><span data-stu-id="82151-137">Request</span></span>
<span data-ttu-id="82151-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82151-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82151-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="82151-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="82151-140">C#</span><span class="sxs-lookup"><span data-stu-id="82151-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82151-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82151-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82151-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82151-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82151-143">响应</span><span class="sxs-lookup"><span data-stu-id="82151-143">Response</span></span>
<span data-ttu-id="82151-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82151-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
